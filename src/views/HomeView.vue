<script setup lang="ts">
import Logo from "../components/Logo.vue";
import MenuIcon from "../assets/menu-burger.svg";
import SearchIcon from "../assets/search.svg";
import SpeakerIcon from "../assets/speaker.b9a3467f.svg";
import ArrowRightIcon from "../assets/arrow-right.svg";
import Section1 from "@/components/Section1.vue";
// import TheWelcome from '../components/TheWelcome.vue'

const title = "Bybit";
</script>

<template>
  <div class="h-[100vh]">
    <!-- 头部 -->
    <header
      class="h-[48px] text-white flex flex-nowrap justify-between items-center px-3"
      style="background-color: #17181e"
    >
      <!-- header left -->
      <div class="flex">
        <!-- logo -->
        <div class="h-[22px]">
          <Logo />
        </div>
      </div>
      <!-- 右边Item -->
      <div class="h-full flex justify-end items-center">
        <img :src="SearchIcon" alt="search" class="h-[16px] text-white mr-6" />
        <img :src="MenuIcon" class="h-[16px]" alt="memu" />
      </div>
    </header>
    <!-- 幻灯片 -->
    <div class="h-[140px] bg-[url('../assets/banner.jpeg')] flex flex-col justify-center items-center gap-2 relative">
      <!-- 描述 -->
      <span class="bg-gradient-to-r from-[#ffd748] to-[#f7a600] bg-clip-text text-transparent font-bold text-[28px]">
        {{ title }} Copy Trading
      </span>
      <span class="text-white text-[14px] font-semibold">32M+ successful trades, 75% win rate</span>
      <!-- 幻灯片 -->
      <div class="carousel w-full h-full absolute">
        <div id="slide1" class="carousel-item relative w-full">
          <img src="https://daisyui.com/images/stock/photo-1625726411847-8cbb60cc71e6.jpg" class="w-full" />
          <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
            <a href="#slide4" class="btn btn-circle">❮</a>
            <a href="#slide2" class="btn btn-circle">❯</a>
          </div>
        </div>
        <div id="slide2" class="carousel-item relative w-full">
          <img src="https://daisyui.com/images/stock/photo-1609621838510-5ad474b7d25d.jpg" class="w-full" />
          <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
            <a href="#slide1" class="btn btn-circle">❮</a>
            <a href="#slide3" class="btn btn-circle">❯</a>
          </div>
        </div>
        <div id="slide3" class="carousel-item relative w-full">
          <img src="https://daisyui.com/images/stock/photo-1414694762283-acccc27bca85.jpg" class="w-full" />
          <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
            <a href="#slide2" class="btn btn-circle">❮</a>
            <a href="#slide4" class="btn btn-circle">❯</a>
          </div>
        </div>
        <div id="slide4" class="carousel-item relative w-full">
          <img src="https://daisyui.com/images/stock/photo-1665553365602-b2fb8e5d1707.jpg" class="w-full" />
          <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
            <a href="#slide3" class="btn btn-circle">❮</a>
            <a href="#slide1" class="btn btn-circle">❯</a>
          </div>
        </div>
      </div>
    </div>
    <!-- 通知栏 -->
    <div class="">
      <div class="h-[32px] flex justify-around items-center bg-white px-3">
        <img class="h-[16px]" :src="SpeakerIcon" alt="SpeakerIcon" />
        <!-- 文本通知 -->
        <span class="w-10/12 text-sm tracking-tight font-medium text-[#121214]">
          Next Up on {{ title }}: Oct 16, 2023 – Oct 29, 2023
        </span>
        <img class="h-[28px]" :src="ArrowRightIcon" alt="ArrowRightIcon" />
      </div>
    </div>
    <!-- 主体展示区域 -->
    <main class="bg-white">
      <!-- 栏目一 -->
      <Section1 />
    </main>
  </div>
</template>
