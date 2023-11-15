<script setup lang="ts">
import rankBg1 from "../assets/rank_bg1.png";
import rankBg2 from "../assets/rank_bg2.png";
import rankBg3 from "../assets/rank_bg3.png";
import rankBg4 from "../assets/rank_bg4.png";
import Up from "../assets/caret-up.svg";
import Down from "../assets/caret-down.svg";
import LevelItem from "./LevelItem.vue";
import { computed, onMounted, ref } from "vue";
import { createChart, ColorType } from "lightweight-charts";

/**
 * 排行容器
 * 注意事项:
 * 1.
 */
export type RankItemType = {
  logo: string;
  title: string;
  level: number;
  follows: number;
  rate: { type: "up" | "down"; value: string };
  offline: boolean;
  roi: { "7d": string; "90d": string }; // 7d, 30d...
  drawdown: string;
  aum: string;
  url: string;
  dataList: number[];
};

// 属性
const props = defineProps<RankItemType & { index: number }>();

const mainRoi = computed(() => {
  const obj = Object.entries(props.roi)[0];
  return {
    type: obj[0],
    value: obj[1],
  };
});
const secondRoi = computed(() => {
  const obj = Object.entries(props.roi)[1];
  return {
    type: obj[0],
    value: obj[1],
  };
});

// 排行icon
function getRankKind(index: number) {
  switch (props.index) {
    case 0:
      return rankBg4;
    case 1:
      return rankBg3;
    case 2:
      return rankBg2;
    default:
      return rankBg1;
  }
}

// 点击操作
const onClick = () => {};

// canvas渲染容器
const canvas = ref<HTMLDivElement>();

// 挂载后 hooks
onMounted(() => {
  if (canvas.value) {
    const chart = createChart(canvas.value, {
      layout: { textColor: "black", background: { type: ColorType.Solid, color: "white" } },
      timeScale: { visible: false },
      grid: { horzLines: { visible: false }, vertLines: { visible: false } },
      rightPriceScale: { visible: false },
      handleScroll: false,
      handleScale: false,
      width: 150,
    });
    // change default top & bottom colors of an area series in creating time
    const areaSeries = chart.addAreaSeries({
      lineColor: "#20b26c",
      lineWidth: 1,
      topColor: "rgba(32, 178, 108, 0.59)",
      bottomColor: "rgba(32, 178, 108, 0)",
      baseLineVisible: true,
    });

    areaSeries.setData(
      props.dataList.map((v, k) => ({
        value: v,
        time: k as any,
      }))
    );

    chart.timeScale().fitContent();
  }
});
</script>

<template>
  <div class="bg-white">
    <!-- 头部 -->
    <div class="h-[136.8px] relative overflow-hidden rounded">
      <img
        :src="getRankKind(index)"
        alt="bg"
        class="h-full w-full absolute left-0 top-0 bg-[length:25%_auto] bg-[8.5%_90%] bg-no-repeat"
        :class="props.logo"
      />
      <!-- No.*** -->
      <p
        class="h-10 w-[88px] absolute bg-[#c289004d] rounded-bl-3xl right-0 top-0 flex justify-center items-center font-bold text-white text-lg"
      >
        No.0{{ index + 1 }}
      </p>
      <!-- 标题 -->
      <p class="absolute top-[47%] left-[34%] flex gap-2 items-center h-7">
        <span class="font-semibold text-[#121214] text-xl">{{ props.title }}</span>
        <LevelItem class="" :level="props.level" :offline="props.offline" />
      </p>
      <!-- 下方follow描述 -->
      <p class="absolute top-[70%] left-[34%] flex gap-2 items-center h-7 text-[#121214] text-xs tracking-tighter">
        <span class="">{{ props.follows }} Follower(s)</span>
        <span class="flex items-center">
          <img class="h-5" :src="props.rate.type === 'up' ? Up : Down" alt="up_down" />
          <span class="">{{ props.rate.value }}</span>
        </span>
      </p>
      <p></p>
    </div>
    <div class="px-6">
      <!-- k线 d 展示 -->
      <div class="py-3 flex justify-between">
        <!-- 左边 -->
        <div class="flex flex-col justify-between items-stretch text-gray-400 h-[60px]">
          <span class="space-x-1">
            <span class="text-sm"> ROI </span>
            <span class="text-xs rounded border border-gray-300 px-1"> {{ mainRoi.type }}</span>
          </span>
          <span class="text-2xl text-gray-800">{{ mainRoi.value }}</span>
        </div>
        <!-- 右边 k线 -->
        <div class="w-[144px]" ref="canvas"></div>
      </div>
      <!-- 下方展示 -->
      <div class="text-sm space-y-1">
        <!-- 第一栏 -->
        <div class="flex justify-between items-center">
          <!-- 左边 -->
          <span class="space-x-1 text-gray-400">
            <span class="text-sm"> ROI </span>
            <span class="text-xs rounded border border-gray-300 px-1"> {{ secondRoi.type }}</span>
          </span>
          <!-- 右边 -->
          <span class="text-gray-800">{{ secondRoi.value }}</span>
        </div>
        <!-- 第二栏 -->
        <div class="flex justify-between items-center">
          <!-- 左边 -->
          <span class="space-x-1 text-gray-400">
            <span class="text-sm"> Drawdown </span>
            <span class="text-xs rounded border border-gray-300 px-1"> 30d</span>
          </span>
          <!-- 右边 -->
          <span class="text-gray-800">{{ props.drawdown }}</span>
        </div>
        <!-- 第三栏 -->
        <div class="flex justify-between items-center">
          <!-- 左边 -->
          <span class="space-x-1 text-gray-400">
            <span class="text-sm"> AUM </span>
          </span>
          <!-- 右边 -->
          <span class="text-gray-800">{{ props.aum }}</span>
        </div>
      </div>
      <!-- 按钮 -->
      <button @click="onClick" class="rounded text-gray-800 bg-[#f7a600] w-full py-3 mt-4 mb-5 font-bold tracking-wide">
        Copy
      </button>
    </div>
  </div>
</template>
