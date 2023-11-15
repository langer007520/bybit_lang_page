<script setup lang="ts">
import TopTradeIcon from "../assets/toptrader.svg";
import MenuIcon from "../assets/alltradergray.svg";
import RankItem, { type RankItemType } from "./RankItem.vue";
import { ref } from "vue";
import Game from "./Game.vue";

const rawList: RankItemType[] = [
  {
    logo: "bg-[url('../assets/test.svg')]",
    title: "blackbird",
    level: 5,
    follows: 250,
    rate: {
      type: "down",
      value: "0.35%",
    },
    offline: true,
    roi: {
      "7d": "+304.97%",
      "90d": "+414.10%",
    }, // 7d, 30d...
    drawdown: "29.33%",
    aum: "155,754.75",
    dataList: [1, 2, 3, 5, 10, 15, 30, 46, 80],
    url: "",
  },
  {
    logo: "bg-[url('../assets/p1.avif')]",
    title: "Tank Capital",
    level: 4,
    follows: 5302,
    rate: {
      type: "down",
      value: "0.51%",
    },
    offline: true,
    roi: {
      "7d": "+128.31%",
      "90d": "+721.29%",
    }, // 7d, 30d...
    drawdown: "29.00%",
    aum: "589,324.08",
    dataList: [40, 42, 43, 50, 45, 35, 40, 46, 60],
    url: "",
  },
  {
    logo: "bg-[url('../assets/p2.avif')]",
    title: "Captain Jack",
    level: 3,
    follows: 18638,
    rate: {
      type: "down",
      value: "2.56%",
    },
    offline: true,
    roi: {
      "7d": "+512.20%",
      "90d": "+1103.56%",
    }, // 7d, 30d...
    drawdown: "35.85%",
    aum: "2155,974.02",
    dataList: [10, 20, 23, 25, 15, 25, 30, 46, 80],
    url: "",
  },
  {
    logo: "bg-[url('../assets/p3.avif')]",
    title: "Bond Strategy",
    level: 2,
    follows: 36205,
    rate: {
      type: "down",
      value: "8.91%",
    },
    offline: true,
    roi: {
      "7d": "+523.03%",
      "90d": "+3754.99%",
    }, // 7d, 30d...
    drawdown: "21.85%",
    aum: "7092,428.05",
    dataList: [10, 20, 13, 15, 14, 15, 22, 46, 50],
    url: "",
  },

  {
    logo: "bg-[url('../assets/p4.avif')]",
    title: "Knight Capital",
    level: 1,
    follows: 12508,
    rate: {
      type: "down",
      value: "0.98%",
    },
    offline: true,
    roi: {
      "7d": "+108.67%",
      "90d": "+6414.10%",
    }, // 7d, 30d...
    drawdown: "27.78%",
    aum: "8105,328.89",
    dataList: [1, 1, 10, 5, 0, 15, 10, 16, 15],
    url: "",
  },
  {
    logo: "bg-[url('../assets/p5.avif')]",
    title: "Alpha AI-101",
    level: 6,
    follows: 5908,
    rate: {
      type: "down",
      value: "2.89%",
    },
    offline: true,
    roi: {
      "7d": "+205.90%",
      "90d": "+840.22%",
    }, // 7d, 30d...
    drawdown: "35.23%",
    aum: "385,880.21",
    dataList: [1, 3, 9, 15, 8, 7, 8, 15, 25],
    url: "",
  },
];
const list = rawList.sort((a, b) => b.follows - a.follows);

const index = ref(0);
</script>

<template>
  <div class="sticky z-10 top-0 flex gap-5 bg-white px-3 py-3 border-b border-b-gray-100">
    <div class="flex flex-nowrap items-center gap-2 group" :class="index == 0 ? 'active' : ''" @click="index = 0">
      <img class="h-5 w-5 group-[.active]:filter-none filter grayscale" :src="TopTradeIcon" alt="TopTradeIcon" />
      <span class="text-base font-medium group-[.active]:text-[#121214] text-gray-400">Top Master Traders</span>
    </div>
    <div class="flex flex-nowrap items-center gap-2 group" :class="index == 1 ? 'active' : ''" @click="index = 1">
      <img class="h-4 w-4 group-[.active]:filter-none filter grayscale" :src="MenuIcon" alt="MenuIcon" />
      <span class="text-base font-medium group-[.active]:text-[#121214] text-gray-400">All Master Traders</span>
    </div>
  </div>
  <div class="">
    <!-- 排行榜一 -->
    <div class="px-3" v-if="index == 0">
      <!-- 栏目标题 -->
      <div class="flex flex-col px-3 py-4 gap-1 bg-white">
        <span class="text-xl font-semibold text-[#121214]">Top Traders By ROI</span>
        <span class="text-xs text-gray-500 tracking-tight font-light">
          Traders that have earned the highest ROI in the last 7 days.
        </span>
      </div>
      <!-- 栏目内容 -->
      <div class="px-3 space-y-5">
        <!-- 排行容器 -->
        <RankItem class="shadow" v-for="(item, k) in list" v-bind="item" :index="k" />
      </div>
    </div>
    <!-- 活动 -->
    <div class="bg-[#090404]" v-else>
      <Game />
    </div>
  </div>
</template>
