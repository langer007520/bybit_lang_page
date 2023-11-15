<script setup lang="ts">
import Video from "../assets/kcgi-2023-h5.mp4";
import BorderIcon from "../assets/border.png";
import GameItem from "../components/GameItem.vue";

const list = [
  {
    volume: "15,045,110.75",
    amount: "10,623.66",
    title: "CryptoSquad",
    img: "https://img.bitgetimg.com/multiLang/web/a7992caa12815a8decffe0584899ba33.png",
  },
  {
    volume: "15,045,110.75",
    amount: "10,623.66",
    title: "CryptoSquad",
    img: "https://img.bitgetimg.com/multiLang/web/a7992caa12815a8decffe0584899ba33.png",
  },

  {
    volume: "15,045,110.75",
    amount: "10,623.66",
    title: "CryptoSquad",
    img: "https://img.bitgetimg.com/multiLang/web/a7992caa12815a8decffe0584899ba33.png",
  },
  {
    volume: "15,045,110.75",
    amount: "10,623.66",
    title: "CryptoSquad",
    img: "https://img.bitgetimg.com/multiLang/web/a7992caa12815a8decffe0584899ba33.png",
  },
  {
    volume: "15,045,110.75",
    amount: "10,623.66",
    title: "CryptoSquad",
    img: "https://img.bitgetimg.com/multiLang/web/a7992caa12815a8decffe0584899ba33.png",
  },
  {
    volume: "15,045,110.75",
    amount: "10,623.66",
    title: "CryptoSquad",
    img: "https://img.bitgetimg.com/multiLang/web/a7992caa12815a8decffe0584899ba33.png",
  },
];
</script>

<template>
  <div class="">
    <!-- 头部视频 -->
    <video :src="Video" autoplay loop />
    <!-- 比赛版 -->
    <div class="px-3">
      <!-- 框架 -->
      <div class="mt-6 border-[#08ffff] border-[1px] relative p-3">
        <!-- 四个角 -->
        <img :src="BorderIcon" class="h-[22px] w-[22px] absolute left-[-2px] top-[-2px]" alt="border" />
        <img :src="BorderIcon" class="h-[22px] w-[22px] absolute right-[-2px] top-[-2px] rotate-90" alt="border" />
        <img :src="BorderIcon" class="h-[22px] w-[22px] absolute right-[-2px] bottom-[-2px] rotate-180" alt="border" />
        <img :src="BorderIcon" class="h-[22px] w-[22px] absolute left-[-2px] bottom-[-2px] -rotate-90" alt="border" />
        <!-- 比赛内容 -->
        <h1
          class="text-[#08FFFF] leading-[22px] text-[18px] text-center font-[900] mb-[6px] md:mb-[unset] md:text-[32px] md:leading-[44px]"
        >
          KCGI 2023 overall participants
        </h1>
        <div class="text-[#FEE45B] text-[24px] text-center md:text-[32px] md:leading-[44px]">19,031</div>
        <p class="text-[12px] text-[#fff] text-center leading-[16px] md:text-[16px] md:leading-[22px]">
          We extend our sincere gratitude to all participants. You are the reason behind the success of KCGI 2023!
        </p>
        <div class="mt-[30px] flex flex-wrap even:mr-[8px] -mb-[16px] md:-mb-[60px] md:mt-[64px] 2xl:mt-[76px]">
          <div class="w-[50%] h-[64px] mb-[16px] md:w-[25%] md:h-[100px] md:mb-[40px] md:text-center md:px-[12px]">
            <p
              class="kcgi_alternate__PfGS3 text-[24px] text-[#fff] leading-[28px] font-[700] mb-[4px] md:mb-[12px] md:text-[32px] lg:text-[44px] lg:leading-[40px] 2xl:text-[50px] 2xl:leading-[44px]"
            >
              5,966
            </p>
            <p
              class="kcgi_word_break__3n1kC text-[12px] text-[#A0A5A6] leading-[16px] md:text-[14px] lg:text-[16px] lg:leading-[22px]"
            >
              Spot trading competition participants
            </p>
          </div>
          <div class="w-[50%] h-[64px] mb-[16px] md:w-[25%] md:h-[100px] md:mb-[40px] md:text-center md:px-[12px]">
            <p
              class="kcgi_alternate__PfGS3 text-[24px] text-[#fff] leading-[28px] font-[700] mb-[4px] md:mb-[12px] md:text-[32px] lg:text-[44px] lg:leading-[40px] 2xl:text-[50px] 2xl:leading-[44px]"
            >
              3,733
            </p>
            <p
              class="kcgi_word_break__3n1kC text-[12px] text-[#A0A5A6] leading-[16px] md:text-[14px] lg:text-[16px] lg:leading-[22px]"
            >
              Demo trading competition
            </p>
          </div>
          <div class="w-[50%] h-[64px] mb-[16px] md:w-[25%] md:h-[100px] md:mb-[40px] md:text-center md:px-[12px]">
            <p
              class="kcgi_alternate__PfGS3 text-[24px] text-[#fff] leading-[28px] font-[700] mb-[4px] md:mb-[12px] md:text-[32px] lg:text-[44px] lg:leading-[40px] 2xl:text-[50px] 2xl:leading-[44px]"
            >
              1,070
            </p>
            <p
              class="kcgi_word_break__3n1kC text-[12px] text-[#A0A5A6] leading-[16px] md:text-[14px] lg:text-[16px] lg:leading-[22px]"
            >
              Futures copy trading competition participants
            </p>
          </div>
          <div class="w-[50%] h-[64px] mb-[16px] md:w-[25%] md:h-[100px] md:mb-[40px] md:text-center md:px-[12px]">
            <p
              class="kcgi_alternate__PfGS3 text-[24px] text-[#fff] leading-[28px] font-[700] mb-[4px] md:mb-[12px] md:text-[32px] lg:text-[44px] lg:leading-[40px] 2xl:text-[50px] 2xl:leading-[44px]"
            >
              10,234
            </p>
            <p
              class="kcgi_word_break__3n1kC text-[12px] text-[#A0A5A6] leading-[16px] md:text-[14px] lg:text-[16px] lg:leading-[22px]"
            >
              Futures trading team battle
            </p>
          </div>
          <div class="w-[50%] h-[64px] mb-[16px] md:w-[25%] md:h-[100px] md:mb-[40px] md:text-center md:px-[12px]">
            <p
              class="kcgi_alternate__PfGS3 text-[24px] text-[#fff] leading-[28px] font-[700] mb-[4px] md:mb-[12px] md:text-[32px] lg:text-[44px] lg:leading-[40px] 2xl:text-[50px] 2xl:leading-[44px]"
            >
              4,525
            </p>
            <p
              class="kcgi_word_break__3n1kC text-[12px] text-[#A0A5A6] leading-[16px] md:text-[14px] lg:text-[16px] lg:leading-[22px]"
            >
              Individual futures trading competition participants
            </p>
          </div>
          <div class="w-[50%] h-[64px] mb-[16px] md:w-[25%] md:h-[100px] md:mb-[40px] md:text-center md:px-[12px]">
            <p
              class="kcgi_alternate__PfGS3 text-[24px] text-[#fff] leading-[28px] font-[700] mb-[4px] md:mb-[12px] md:text-[32px] lg:text-[44px] lg:leading-[40px] 2xl:text-[50px] 2xl:leading-[44px]"
            >
              4,694
            </p>
            <p
              class="kcgi_word_break__3n1kC text-[12px] text-[#A0A5A6] leading-[16px] md:text-[14px] lg:text-[16px] lg:leading-[22px]"
            >
              Number of referrals
            </p>
          </div>
          <div class="w-[50%] h-[64px] mb-[16px] md:w-[25%] md:h-[100px] md:mb-[40px] md:text-center md:px-[12px]">
            <p
              class="kcgi_alternate__PfGS3 text-[24px] text-[#fff] leading-[28px] font-[700] mb-[4px] md:mb-[12px] md:text-[32px] lg:text-[44px] lg:leading-[40px] 2xl:text-[50px] 2xl:leading-[44px]"
            >
              14,636
            </p>
            <p
              class="kcgi_word_break__3n1kC text-[12px] text-[#A0A5A6] leading-[16px] md:text-[14px] lg:text-[16px] lg:leading-[22px]"
            >
              Lucky Draw participants
            </p>
          </div>
        </div>
      </div>
      <!-- 排行榜 -->
      <div class="mt-3">
        <!-- 头 -->
        <div class="relative">
          <img src="../assets/title-h5.png" alt="title" class="mx-auto absolute inset-x-0 top-0" />
          <p class="w-1/2 mx-auto text-center text-[#FFFFFF] text-[13px] font-[700] leading-[26px]">
            Top 10 of the spot trading competition
          </p>
          <div class="grid gap-3">
            <GameItem v-for="(item, k) in list" v-bind="item" :index="k" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
