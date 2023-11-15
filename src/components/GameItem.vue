<script setup lang="ts">
/**
 * 比赛排行版 item
 */

defineProps<{
  index: number;
  amount: string;
  volume: string;
  img: string;
  title: string;
}>();
</script>

<template>
  <div class="border-[#00FFF1] border-[0.5px] rounded-[8px] px-3 flex gap-3">
    <img
      :src="img"
      class="border-[1px] border-solid border-[#fff] block w-[24px] h-[24px] rounded-[99px] mt-3"
      alt=""
    />
    <div class="flex-1">
      <div class="flex justify-between items-center">
        <span class="truncate text-[#fff] text-[16px] leading-[48px]">{{ title }}</span>
        <svg
          width="1em"
          height="1em"
          viewBox="0 0 280 272"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="w-[48px] h-[48px]"
          v-if="index == 0"
        >
          <g filter="url(#prize-1_svg__a)">
            <path
              d="M44.46 149.438c-.597-3.926 2.748-7.335 6.687-6.816l88.177 11.621a5.937 5.937 0 0 1 5.139 6.416l-1.406 15.814a5.98 5.98 0 0 1-6.751 5.392l-84.33-11.39a5.935 5.935 0 0 1-5.078-4.991l-2.439-16.046Z"
              fill="#FF7B01"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__b)">
            <path
              d="M25.467 129.193c-.596-3.925 2.748-7.335 6.687-6.815l88.177 11.621a5.937 5.937 0 0 1 5.14 6.416l-1.407 15.814a5.978 5.978 0 0 1-6.75 5.392l-84.331-11.39a5.935 5.935 0 0 1-5.077-4.992l-2.439-16.046Z"
              fill="#FFA001"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__c)">
            <path
              d="M6.999 103.169c-.597-3.926 2.748-7.335 6.687-6.816l88.177 11.622a5.937 5.937 0 0 1 5.14 6.415l-1.407 15.815a5.978 5.978 0 0 1-6.75 5.391l-84.332-11.39a5.935 5.935 0 0 1-5.077-4.991L7 103.169Z"
              fill="#FECC50"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__d)">
            <path
              d="M233.798 149.451c.597-3.926-2.748-7.335-6.687-6.816l-88.177 11.622a5.937 5.937 0 0 0-5.14 6.416l1.407 15.814a5.979 5.979 0 0 0 6.75 5.392l84.332-11.39a5.937 5.937 0 0 0 5.076-4.992l2.439-16.046Z"
              fill="#FF7B01"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__e)">
            <path
              d="M252.783 129.193c.596-3.925-2.748-7.335-6.687-6.815l-88.177 11.621a5.937 5.937 0 0 0-5.14 6.416l1.407 15.814a5.978 5.978 0 0 0 6.75 5.392l84.331-11.39a5.935 5.935 0 0 0 5.077-4.992l2.439-16.046Z"
              fill="#FFA001"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__f)">
            <path
              d="M271.251 103.169c.597-3.926-2.748-7.335-6.687-6.816l-88.177 11.622a5.937 5.937 0 0 0-5.14 6.415l1.407 15.815a5.978 5.978 0 0 0 6.751 5.391l84.331-11.39a5.937 5.937 0 0 0 5.077-4.991l2.438-16.046Z"
              fill="#FECC50"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__g)">
            <mask
              id="prize-1_svg__h"
              maskUnits="userSpaceOnUse"
              x="111"
              y="76"
              width="58"
              height="58"
              style="mask-type: alpha"
            >
              <path
                d="M128.285 81.23c6.505-6.396 16.937-6.396 23.442 0l6.161 6.06 5.762 5.666c6.661 6.55 6.661 17.287 0 23.837l-5.762 5.667-6.161 6.058c-6.505 6.397-16.937 6.397-23.442 0l-6.161-6.058-5.762-5.667c-6.66-6.55-6.66-17.287 0-23.837l5.762-5.667 6.161-6.059Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-1_svg__h)" fill="#FFD0F5">
              <path d="m211.533 140.045-35.764-35.171-35.764 35.171h71.528Z"></path>
              <path d="M68.477 140.045h71.528l-35.764-35.171-35.764 35.171Z"></path>
            </g>
          </g>
          <g filter="url(#prize-1_svg__i)">
            <mask
              id="prize-1_svg__j"
              maskUnits="userSpaceOnUse"
              x="147"
              y="111"
              width="58"
              height="58"
              style="mask-type: alpha"
            >
              <path
                d="M199.481 128.058c6.661 6.55 6.661 17.288 0 23.838l-5.762 5.666-6.161 6.059c-6.504 6.397-16.937 6.397-23.442 0l-6.161-6.059-5.762-5.666c-6.66-6.55-6.66-17.288 0-23.838l5.762-5.666 6.161-6.059c6.505-6.397 16.938-6.397 23.442 0l6.161 6.059 5.762 5.666Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-1_svg__j)" fill="#FFD0F5">
              <path d="m140.073 210.313 35.764-35.17-35.764-35.171v70.341Z"></path>
              <path d="M140.073 69.632v70.34l35.764-35.17-35.764-35.17Z"></path>
            </g>
          </g>
          <g filter="url(#prize-1_svg__k)">
            <mask
              id="prize-1_svg__l"
              maskUnits="userSpaceOnUse"
              x="111"
              y="146"
              width="58"
              height="58"
              style="mask-type: alpha"
            >
              <path
                d="M151.863 198.853c-6.505 6.396-16.937 6.396-23.442 0l-6.161-6.059-5.762-5.667c-6.661-6.55-6.661-17.287 0-23.837l5.762-5.667 6.161-6.058c6.505-6.397 16.937-6.397 23.442 0l6.161 6.058 5.762 5.667c6.661 6.55 6.661 17.287 0 23.837l-5.762 5.667-6.161 6.059Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-1_svg__l)" fill="#FFD0F5">
              <path
                d="m68.615 140.038 35.764 35.171 35.765-35.171H68.615ZM211.672 140.038h-71.528l35.764 35.171 35.764-35.171Z"
              ></path>
            </g>
          </g>
          <g filter="url(#prize-1_svg__m)">
            <mask
              id="prize-1_svg__n"
              maskUnits="userSpaceOnUse"
              x="75"
              y="111"
              width="58"
              height="58"
              style="mask-type: alpha"
            >
              <path
                d="M80.667 152.027c-6.66-6.55-6.66-17.288 0-23.838l5.762-5.666 6.161-6.059c6.505-6.397 16.937-6.397 23.442 0l6.161 6.059 5.762 5.666c6.661 6.55 6.661 17.288 0 23.838l-5.762 5.666-6.161 6.059c-6.505 6.397-16.937 6.397-23.442 0l-6.161-6.059-5.762-5.666Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-1_svg__n)">
              <path d="m140.075 69.772-35.764 35.17 35.764 35.171V69.772Z" fill="#FFD0F5"></path>
            </g>
          </g>
          <path d="m138.354 42.226 28.994 33.119H109.36l28.994-33.12Z" fill="url(#prize-1_svg__o)"></path>
          <path d="m138.357 231.226-28.994-33.12h57.988l-28.994 33.12Z" fill="url(#prize-1_svg__p)"></path>
          <g filter="url(#prize-1_svg__q)">
            <path
              d="m138.362 51.065 3.359 9.969 10.213 3.278-10.213 3.279-3.359 9.969-3.359-9.97-10.214-3.278 10.214-3.278 3.359-9.97Z"
              fill="#fff"
            ></path>
            <path
              d="m138.362 51.39 3.26 9.677.017.05.05.015 9.906 3.18-9.906 3.18-.05.016-.017.05-3.26 9.677-3.261-9.677-.017-.05-.05-.016-9.906-3.18 9.906-3.18.05-.016.017-.05 3.261-9.677Z"
              stroke="#FAFF00"
              stroke-width="0.207"
            ></path>
          </g>
          <path d="m222.198 183.977-43.883 7.949 28.994-49.016 14.889 41.067Z" fill="url(#prize-1_svg__r)"></path>
          <path d="m54.505 89.474 43.883-7.949-28.994 49.017-14.889-41.068Z" fill="url(#prize-1_svg__s)"></path>
          <path d="m222.201 89.478-14.889 41.067-28.994-49.016 43.883 7.949Z" fill="url(#prize-1_svg__t)"></path>
          <path d="M54.51 183.974 69.4 142.906l28.994 49.016-43.883-7.948Z" fill="url(#prize-1_svg__u)"></path>
          <path
            d="M212.938 135.849c0 39.699-32.975 71.902-73.678 71.902-40.704 0-73.679-32.203-73.679-71.902 0-39.7 32.975-71.903 73.679-71.903 40.703 0 73.678 32.204 73.678 71.903Z"
            fill="url(#prize-1_svg__v)"
            stroke="url(#prize-1_svg__w)"
            stroke-width="1.037"
          ></path>
          <g filter="url(#prize-1_svg__x)">
            <ellipse cx="139.25" cy="135.841" rx="65.149" ry="63.589" fill="url(#prize-1_svg__y)"></ellipse>
          </g>
          <g filter="url(#prize-1_svg__z)">
            <ellipse cx="139.259" cy="135.846" rx="54.291" ry="52.991" fill="url(#prize-1_svg__A)"></ellipse>
          </g>
          <path
            d="M122.472 129.05v-11.439l16.371-9.15h9.579v52.401h-12.367v-39.319l-13.583 7.507ZM110.304 89.913l1.344 3.988 4.085 1.311-4.085 1.312-1.344 3.987-1.344-3.987-4.085-1.312 4.085-1.311 1.344-3.988ZM94.02 72.252l3.135 9.304 9.532 3.06-9.532 3.06-3.136 9.305-3.135-9.304-9.532-3.06 9.532-3.06 3.135-9.305Z"
            fill="#fff"
          ></path>
          <defs>
            <filter
              id="prize-1_svg__a"
              x="10.958"
              y="142.569"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.11 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__b"
              x="-8.034"
              y="122.325"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.19 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__c"
              x="-26.503"
              y="96.301"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.42 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__d"
              x="100.341"
              y="142.583"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.11 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__e"
              x="119.325"
              y="122.325"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.19 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__f"
              x="137.794"
              y="96.301"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.42 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__g"
              x="44.502"
              y="38.008"
              width="191.012"
              height="162.174"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="33.433"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__i"
              x="80.33"
              y="44.67"
              width="162.372"
              height="190.615"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="33.433"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__k"
              x="44.634"
              y="79.901"
              width="191.012"
              height="162.174"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="33.433"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__m"
              x="37.447"
              y="44.8"
              width="162.372"
              height="162.177"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="33.433"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__q"
              x="121.678"
              y="47.953"
              width="33.371"
              height="32.718"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feGaussianBlur stdDeviation="1.556" result="effect1_foregroundBlur_5589_132916"></feGaussianBlur>
            </filter>
            <filter
              id="prize-1_svg__x"
              x="74.102"
              y="70.178"
              width="130.297"
              height="129.253"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="-2.074"></feOffset>
              <feGaussianBlur stdDeviation="1.037"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0.616667 0 0 0 0 0.407 0 0 0 0 0 0 0 0 0.25 0"></feColorMatrix>
              <feBlend in2="shape" result="effect1_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__z"
              x="84.969"
              y="80.781"
              width="108.578"
              height="110.131"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="2.074"></feOffset>
              <feGaussianBlur stdDeviation="2.074"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0.7 0 0 0 0 0.465967 0 0 0 0 0.0116667 0 0 0 1 0"></feColorMatrix>
              <feBlend in2="shape" result="effect1_innerShadow_5589_132916"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="-2.074"></feOffset>
              <feGaussianBlur stdDeviation="1.037"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 1 0 0 0 0 0.72 0 0 0 0 0 0 0 0 1 0"></feColorMatrix>
              <feBlend in2="effect1_innerShadow_5589_132916" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <linearGradient
              id="prize-1_svg__o"
              x1="126.302"
              y1="55.473"
              x2="150.407"
              y2="55.473"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__p"
              x1="150.409"
              y1="217.978"
              x2="126.304"
              y2="217.978"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__r"
              x1="216.47"
              y1="167.166"
              x2="204.85"
              y2="187.785"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__s"
              x1="60.233"
              y1="106.285"
              x2="71.853"
              y2="85.666"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__t"
              x1="204.42"
              y1="85.913"
              x2="216.04"
              y2="106.533"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__u"
              x1="72.291"
              y1="187.538"
              x2="60.671"
              y2="166.918"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__v"
              x1="91.697"
              y1="81.997"
              x2="187.977"
              y2="192.019"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#FFECA9"></stop>
              <stop offset="0.237" stop-color="#FFD600"></stop>
              <stop offset="1" stop-color="#F90"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__w"
              x1="139.26"
              y1="63.428"
              x2="139.26"
              y2="208.27"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#fff" stop-opacity="0.5"></stop>
              <stop offset="1" stop-color="#fff" stop-opacity="0"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__y"
              x1="97.627"
              y1="87.266"
              x2="178.493"
              y2="187.225"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#FFC700"></stop>
              <stop offset="1" stop-color="#D58500"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__A"
              x1="103.332"
              y1="92.207"
              x2="146.271"
              y2="189.618"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#FFB13C"></stop>
              <stop offset="0.484" stop-color="#B45F1D"></stop>
              <stop offset="1" stop-color="#743110"></stop>
            </linearGradient>
          </defs>
        </svg>
        <svg
          width="1em"
          height="1em"
          viewBox="0 0 200 201"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="w-[48px] h-[48px]"
          v-else-if="index == 1"
        >
          <g clip-path="url(#prize-2_svg__a)">
            <g filter="url(#prize-2_svg__b)">
              <path
                d="M31.774 104.798c-.433-2.806 1.96-5.254 4.779-4.888l62.963 8.172a4.227 4.227 0 0 1 3.669 4.577l-.994 10.996a4.283 4.283 0 0 1-4.825 3.857l-60.247-8.014a4.224 4.224 0 0 1-3.623-3.545l-1.722-11.155Z"
                fill="#A0B0D1"
              ></path>
            </g>
            <g filter="url(#prize-2_svg__c)">
              <path
                d="M18.211 90.558c-.433-2.807 1.96-5.255 4.78-4.889l62.962 8.173a4.226 4.226 0 0 1 3.67 4.577l-.994 10.996a4.284 4.284 0 0 1-4.825 3.857l-60.248-8.014a4.225 4.225 0 0 1-3.623-3.545l-1.722-11.155Z"
                fill="#B5C3E0"
              ></path>
            </g>
            <g filter="url(#prize-2_svg__d)">
              <path
                d="M5.016 72.25c-.433-2.807 1.96-5.255 4.78-4.89l62.962 8.173a4.227 4.227 0 0 1 3.669 4.577l-.994 10.996a4.284 4.284 0 0 1-4.824 3.857L10.36 86.95a4.225 4.225 0 0 1-3.623-3.546L5.016 72.25Z"
                fill="#CBD5E9"
              ></path>
            </g>
            <g filter="url(#prize-2_svg__e)">
              <path
                d="M166.984 104.798c.433-2.806-1.96-5.254-4.779-4.888l-62.963 8.172a4.227 4.227 0 0 0-3.669 4.577l.994 10.996a4.284 4.284 0 0 0 4.824 3.857l60.248-8.014a4.223 4.223 0 0 0 3.623-3.545l1.722-11.155Z"
                fill="#A0B0D1"
              ></path>
            </g>
            <g filter="url(#prize-2_svg__f)">
              <path
                d="M180.546 90.558c.434-2.807-1.96-5.255-4.779-4.889l-62.962 8.173a4.226 4.226 0 0 0-3.669 4.577l.993 10.996a4.284 4.284 0 0 0 4.825 3.857l60.248-8.014a4.226 4.226 0 0 0 3.623-3.545l1.721-11.155Z"
                fill="#B5C3E0"
              ></path>
            </g>
            <g filter="url(#prize-2_svg__g)">
              <path
                d="M193.742 72.25c.433-2.807-1.96-5.255-4.779-4.89L126 75.534a4.226 4.226 0 0 0-3.669 4.577l.993 10.996a4.284 4.284 0 0 0 4.825 3.857l60.248-8.013a4.224 4.224 0 0 0 3.623-3.546l1.722-11.155Z"
                fill="#DDE6F5"
              ></path>
            </g>
            <g filter="url(#prize-2_svg__h)">
              <mask
                id="prize-2_svg__i"
                maskUnits="userSpaceOnUse"
                x="79"
                y="53"
                width="42"
                height="41"
                style="mask-type: alpha"
              >
                <path
                  d="M91.7 56.658c4.63-4.483 11.983-4.483 16.613 0l4.467 4.326 3.915 3.792c4.846 4.692 4.846 12.463 0 17.155l-3.915 3.792-4.467 4.325c-4.63 4.484-11.983 4.484-16.613 0l-4.466-4.325-3.916-3.792c-4.845-4.692-4.845-12.463 0-17.155l3.916-3.792 4.466-4.326Z"
                  fill="#C4C4C4"
                ></path>
              </mask>
              <g mask="url(#prize-2_svg__i)" fill="#FFD0F5">
                <path
                  d="m151.097 98.093-25.545-24.74-25.546 24.74h51.091ZM48.914 98.093h51.092L74.46 73.353l-25.546 24.74Z"
                ></path>
              </g>
            </g>
            <g filter="url(#prize-2_svg__j)">
              <mask
                id="prize-2_svg__k"
                maskUnits="userSpaceOnUse"
                x="105"
                y="77"
                width="41"
                height="42"
                style="mask-type: alpha"
              >
                <path
                  d="M142.291 89.47c4.845 4.692 4.845 12.463 0 17.155l-3.915 3.792-4.467 4.326c-4.63 4.483-11.983 4.483-16.613 0l-4.466-4.326-3.916-3.792c-4.845-4.692-4.845-12.463 0-17.155l3.916-3.792 4.466-4.325c4.63-4.484 11.983-4.484 16.613 0l4.467 4.325 3.915 3.792Z"
                  fill="#C4C4C4"
                ></path>
              </mask>
              <g mask="url(#prize-2_svg__k)" fill="#FFD0F5">
                <path
                  d="m100.057 147.529 25.546-24.739-25.546-24.74v49.479ZM100.057 48.572V98.05l25.546-24.739-25.546-24.739Z"
                ></path>
              </g>
            </g>
            <g filter="url(#prize-2_svg__l)">
              <mask
                id="prize-2_svg__m"
                maskUnits="userSpaceOnUse"
                x="79"
                y="102"
                width="42"
                height="41"
                style="mask-type: alpha"
              >
                <path
                  d="M108.409 139.529c-4.63 4.484-11.983 4.484-16.613 0l-4.466-4.325-3.916-3.792c-4.845-4.692-4.845-12.463 0-17.155l3.916-3.792 4.466-4.326c4.63-4.484 11.983-4.484 16.613 0l4.467 4.326 3.915 3.792c4.845 4.692 4.845 12.463 0 17.155l-3.915 3.792-4.467 4.325Z"
                  fill="#C4C4C4"
                ></path>
              </mask>
              <g mask="url(#prize-2_svg__m)" fill="#FFD0F5">
                <path
                  d="m49.012 98.095 25.546 24.739 25.546-24.739H49.012ZM151.195 98.095h-51.091l25.545 24.739 25.546-24.739Z"
                ></path>
              </g>
            </g>
            <g filter="url(#prize-2_svg__n)">
              <mask
                id="prize-2_svg__o"
                maskUnits="userSpaceOnUse"
                x="54"
                y="78"
                width="41"
                height="41"
                style="mask-type: alpha"
              >
                <path
                  d="M57.818 106.717c-4.845-4.692-4.845-12.463 0-17.155l3.916-3.792 4.466-4.325c4.63-4.484 11.983-4.484 16.613 0l4.467 4.325 3.915 3.792c4.846 4.692 4.846 12.463 0 17.155l-3.915 3.792-4.467 4.326c-4.63 4.484-11.983 4.484-16.613 0l-4.466-4.326-3.916-3.792Z"
                  fill="#C4C4C4"
                ></path>
              </mask>
              <g mask="url(#prize-2_svg__o)">
                <path d="M100.053 48.659 74.507 73.398l25.546 24.739V48.659Z" fill="#FFD0F5"></path>
              </g>
            </g>
            <path d="m100.276 33.154 21.03 23.657h-42.06l21.03-23.657Z" fill="url(#prize-2_svg__p)"></path>
            <path d="m100.279 168.154-21.03-23.656h42.06l-21.03 23.656Z" fill="url(#prize-2_svg__q)"></path>
            <g filter="url(#prize-2_svg__r)">
              <path
                d="m99.696 39.21 2.437 7.122 7.408 2.342-7.408 2.342-2.437 7.12-2.436-7.12-7.408-2.342 7.408-2.342 2.436-7.121Z"
                fill="#fff"
              ></path>
              <path
                d="m99.696 39.44 2.367 6.916.012.035.035.011 7.185 2.272-7.185 2.27-.035.012-.012.035-2.367 6.916-2.366-6.915-.012-.036-.036-.011-7.185-2.271 7.185-2.272.036-.01.012-.036 2.366-6.916Z"
                stroke="#3E74FF"
                stroke-width="0.148"
              ></path>
            </g>
            <path d="m161.085 134.406-31.83 5.677 21.031-35.012 10.799 29.335Z" fill="url(#prize-2_svg__s)"></path>
            <path d="m39.454 66.903 31.83-5.678-21.03 35.012-10.8-29.334Z" fill="url(#prize-2_svg__t)"></path>
            <path d="M161.087 66.906 150.288 96.24l-21.03-35.012 31.829 5.678Z" fill="url(#prize-2_svg__u)"></path>
            <path d="m39.452 134.403 10.8-29.334 21.03 35.012-31.83-5.678Z" fill="url(#prize-2_svg__v)"></path>
            <path
              d="M154.382 100.02c0 28.351-23.916 51.359-53.447 51.359-29.532 0-53.447-23.008-53.447-51.359 0-28.35 23.915-51.359 53.447-51.359 29.531 0 53.447 23.008 53.447 51.359Z"
              fill="url(#prize-2_svg__w)"
              stroke="url(#prize-2_svg__x)"
              stroke-width="0.741"
            ></path>
            <g filter="url(#prize-2_svg__y)">
              <ellipse cx="100.926" cy="100.022" rx="47.254" ry="45.421" fill="url(#prize-2_svg__z)"></ellipse>
            </g>
            <g filter="url(#prize-2_svg__A)">
              <ellipse cx="100.933" cy="100.026" rx="39.379" ry="37.851" fill="url(#prize-2_svg__B)"></ellipse>
            </g>
            <path
              d="M101.669 109.896h14.094v7.557H89.108v-5.668l10.927-12.306c1.805-2.043 3.064-3.626 3.779-4.75.715-1.123 1.072-2.263 1.072-3.42 0-1.158-.323-2.111-.97-2.86-.647-.75-1.549-1.124-2.706-1.124-2.587 0-4.46 1.873-5.617 5.617l-6.74-3.931c.953-3.132 2.604-5.532 4.953-7.2 2.348-1.669 5.089-2.503 8.221-2.503 2.553 0 4.732.511 6.536 1.532 1.838 1.022 3.217 2.417 4.136 4.188.919 1.736 1.379 3.676 1.379 5.82 0 2.145-.511 4.137-1.532 5.975-1.021 1.805-2.843 4.136-5.464 6.996l-5.413 6.077ZM79.93 67.217l.975 2.848 2.963.937-2.963.937-.975 2.848-.975-2.848-2.963-.937 2.963-.937.975-2.848ZM68.11 54.602l2.274 6.646 6.915 2.185-6.915 2.186-2.274 6.646-2.274-6.646-6.914-2.186 6.914-2.185 2.274-6.646Z"
              fill="#fff"
            ></path>
          </g>
          <defs>
            <filter
              id="prize-2_svg__b"
              x="7.846"
              y="99.873"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.11 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132897"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__c"
              x="-5.717"
              y="85.633"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.19 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132897"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__d"
              x="-18.912"
              y="67.324"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.42 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132897"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__e"
              x="71.674"
              y="99.873"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.11 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132897"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__f"
              x="85.237"
              y="85.633"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.19 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132897"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__g"
              x="98.432"
              y="67.324"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.42 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132897"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__h"
              x="31.926"
              y="25.592"
              width="136.163"
              height="115.58"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="23.881"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__j"
              x="57.52"
              y="30.229"
              width="115.843"
              height="135.638"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="23.881"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__l"
              x="32.02"
              y="55.015"
              width="136.163"
              height="115.58"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="23.881"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__n"
              x="26.747"
              y="30.321"
              width="115.843"
              height="115.577"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="23.881"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132897"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132897" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__r"
              x="86.148"
              y="35.507"
              width="27.095"
              height="26.334"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feGaussianBlur stdDeviation="1.852" result="effect1_foregroundBlur_5589_132897"></feGaussianBlur>
            </filter>
            <filter
              id="prize-2_svg__y"
              x="53.672"
              y="53.12"
              width="94.508"
              height="92.323"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="-1.482"></feOffset>
              <feGaussianBlur stdDeviation="1.482"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0.172667 0 0 0 0 0.616667 0 0 0 0.15 0"></feColorMatrix>
              <feBlend in2="shape" result="effect1_innerShadow_5589_132897"></feBlend>
            </filter>
            <filter
              id="prize-2_svg__A"
              x="61.555"
              y="60.694"
              width="78.758"
              height="78.664"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="1.482"></feOffset>
              <feGaussianBlur stdDeviation="3.704"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0.193203 0 0 0 0 0.4875 0 0 0 1 0"></feColorMatrix>
              <feBlend in2="shape" result="effect1_innerShadow_5589_132897"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="-1.482"></feOffset>
              <feGaussianBlur stdDeviation="3.704"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0.4375 0 0 0 0 0.62875 0 0 0 0 1 0 0 0 1 0"></feColorMatrix>
              <feBlend in2="effect1_innerShadow_5589_132897" result="effect2_innerShadow_5589_132897"></feBlend>
            </filter>
            <linearGradient
              id="prize-2_svg__p"
              x1="91.534"
              y1="42.617"
              x2="109.018"
              y2="42.617"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#E3EBFF"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#B3C2D9"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__q"
              x1="109.021"
              y1="158.692"
              x2="91.537"
              y2="158.692"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#E3EBFF"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#B3C2D9"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__s"
              x1="156.93"
              y1="122.397"
              x2="148.697"
              y2="137.234"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#E3EBFF"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#B3C2D9"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__t"
              x1="43.609"
              y1="78.912"
              x2="51.842"
              y2="64.075"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#E3EBFF"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#B3C2D9"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__u"
              x1="148.19"
              y1="64.36"
              x2="156.424"
              y2="79.196"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#E3EBFF"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#B3C2D9"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__v"
              x1="52.349"
              y1="136.949"
              x2="44.115"
              y2="122.112"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#E3EBFF"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#B3C2D9"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__w"
              x1="66.436"
              y1="61.555"
              x2="135.059"
              y2="141.186"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#D5E3FF"></stop>
              <stop offset="0.521" stop-color="#F0F5FF"></stop>
              <stop offset="1" stop-color="#D0DFFE"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__x"
              x1="100.935"
              y1="48.291"
              x2="100.935"
              y2="151.75"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#fff" stop-opacity="0.5"></stop>
              <stop offset="1" stop-color="#fff" stop-opacity="0"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__z"
              x1="70.736"
              y1="65.326"
              x2="128.306"
              y2="137.589"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#B1CCFF"></stop>
              <stop offset="1" stop-color="#D5E3FF"></stop>
            </linearGradient>
            <linearGradient
              id="prize-2_svg__B"
              x1="74.874"
              y1="68.855"
              x2="105.227"
              y2="138.779"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#D9E6FF"></stop>
              <stop offset="0.484" stop-color="#77A6EC"></stop>
              <stop offset="1" stop-color="#4C82D2"></stop>
            </linearGradient>
            <clipPath id="prize-2_svg__a">
              <path fill="#fff" transform="translate(0 .735)" d="M0 0h200v200H0z"></path>
            </clipPath>
          </defs>
        </svg>
        <svg
          width="1em"
          height="1em"
          viewBox="0 0 200 201"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="w-[48px] h-[48px]"
          v-else-if="index == 2"
        >
          <g filter="url(#prize-3_svg__a)">
            <path
              d="M31.774 110.78c-.433-2.807 1.96-5.255 4.779-4.889l62.963 8.172a4.227 4.227 0 0 1 3.669 4.577l-.994 10.996a4.283 4.283 0 0 1-4.825 3.857L37.12 125.48a4.225 4.225 0 0 1-3.623-3.546l-1.722-11.154Z"
              fill="#FF7B01"
            ></path>
          </g>
          <g filter="url(#prize-3_svg__b)">
            <path
              d="M18.211 96.54c-.433-2.807 1.96-5.255 4.78-4.89l62.962 8.173a4.226 4.226 0 0 1 3.67 4.577l-.994 10.996a4.284 4.284 0 0 1-4.825 3.857l-60.248-8.013a4.226 4.226 0 0 1-3.623-3.546l-1.722-11.155Z"
              fill="#FFA001"
            ></path>
          </g>
          <g filter="url(#prize-3_svg__c)">
            <path
              d="M5.016 78.23c-.433-2.806 1.96-5.254 4.78-4.888l62.962 8.172a4.226 4.226 0 0 1 3.669 4.578l-.994 10.996a4.283 4.283 0 0 1-4.824 3.856L10.36 92.931a4.225 4.225 0 0 1-3.623-3.545L5.016 78.23Z"
              fill="#FECC50"
            ></path>
          </g>
          <g filter="url(#prize-3_svg__d)">
            <path
              d="M166.984 110.78c.433-2.807-1.96-5.255-4.779-4.889l-62.963 8.172a4.227 4.227 0 0 0-3.669 4.577l.994 10.996a4.283 4.283 0 0 0 4.824 3.857l60.248-8.013a4.224 4.224 0 0 0 3.623-3.546l1.722-11.154Z"
              fill="#FF7B01"
            ></path>
          </g>
          <g filter="url(#prize-3_svg__e)">
            <path
              d="M180.546 96.54c.434-2.807-1.96-5.255-4.779-4.89l-62.962 8.173a4.226 4.226 0 0 0-3.669 4.577l.993 10.996a4.284 4.284 0 0 0 4.825 3.857l60.248-8.013a4.227 4.227 0 0 0 3.623-3.546l1.721-11.155Z"
              fill="#FFA001"
            ></path>
          </g>
          <g filter="url(#prize-3_svg__f)">
            <path
              d="M193.742 78.23c.433-2.806-1.96-5.254-4.779-4.888L126 81.514a4.226 4.226 0 0 0-3.669 4.578l.993 10.996a4.283 4.283 0 0 0 4.825 3.856l60.248-8.013a4.224 4.224 0 0 0 3.623-3.545l1.722-11.155Z"
              fill="#FECC50"
            ></path>
          </g>
          <g filter="url(#prize-3_svg__g)">
            <mask
              id="prize-3_svg__h"
              maskUnits="userSpaceOnUse"
              x="79"
              y="59"
              width="42"
              height="41"
              style="mask-type: alpha"
            >
              <path
                d="M91.7 62.639c4.63-4.484 11.983-4.484 16.613 0l4.467 4.325 3.915 3.792c4.846 4.692 4.846 12.463 0 17.155l-3.915 3.792-4.467 4.326c-4.63 4.484-11.983 4.484-16.613 0l-4.466-4.326-3.916-3.792c-4.845-4.692-4.845-12.463 0-17.155l3.916-3.792L91.7 62.64Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-3_svg__h)" fill="#FFD0F5">
              <path
                d="m151.097 104.073-25.545-24.74-25.546 24.74h51.091ZM48.914 104.073h51.092L74.46 79.333l-25.546 24.74Z"
              ></path>
            </g>
          </g>
          <g filter="url(#prize-3_svg__i)">
            <mask
              id="prize-3_svg__j"
              maskUnits="userSpaceOnUse"
              x="105"
              y="83"
              width="41"
              height="42"
              style="mask-type: alpha"
            >
              <path
                d="M142.291 95.453c4.845 4.692 4.845 12.463 0 17.155l-3.915 3.792-4.467 4.325c-4.63 4.484-11.983 4.484-16.613 0l-4.466-4.325-3.916-3.792c-4.845-4.692-4.845-12.463 0-17.155l3.916-3.792 4.466-4.326c4.63-4.484 11.983-4.484 16.613 0l4.467 4.326 3.915 3.792Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-3_svg__j)" fill="#FFD0F5">
              <path d="m100.057 153.511 25.546-24.739-25.546-24.739v49.478Z"></path>
              <path d="M100.057 54.555v49.478l25.546-24.74-25.546-24.738Z"></path>
            </g>
          </g>
          <g filter="url(#prize-3_svg__k)">
            <mask
              id="prize-3_svg__l"
              maskUnits="userSpaceOnUse"
              x="79"
              y="108"
              width="42"
              height="41"
              style="mask-type: alpha"
            >
              <path
                d="M108.409 145.511c-4.63 4.484-11.983 4.484-16.613 0l-4.466-4.325-3.916-3.792c-4.845-4.692-4.845-12.463 0-17.155l3.916-3.792 4.466-4.325c4.63-4.484 11.983-4.484 16.613 0l4.467 4.325 3.915 3.792c4.845 4.692 4.845 12.463 0 17.155l-3.915 3.792-4.467 4.325Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-3_svg__l)" fill="#FFD0F5">
              <path
                d="m49.012 104.077 25.546 24.74 25.546-24.74H49.012ZM151.195 104.077h-51.091l25.545 24.74 25.546-24.74Z"
              ></path>
            </g>
          </g>
          <g filter="url(#prize-3_svg__m)">
            <mask
              id="prize-3_svg__n"
              maskUnits="userSpaceOnUse"
              x="54"
              y="84"
              width="41"
              height="41"
              style="mask-type: alpha"
            >
              <path
                d="M57.818 112.7c-4.845-4.692-4.845-12.463 0-17.155l3.916-3.792 4.466-4.326c4.63-4.484 11.983-4.484 16.613 0l4.467 4.326 3.915 3.792c4.846 4.692 4.846 12.463 0 17.155l-3.915 3.792-4.467 4.325c-4.63 4.484-11.983 4.484-16.613 0l-4.466-4.325-3.916-3.792Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-3_svg__n)">
              <path d="m100.053 54.641-25.546 24.74 25.546 24.738V54.641Z" fill="#FFD0F5"></path>
            </g>
          </g>
          <path d="m99.908 33.502 21.031 23.657h-42.06l21.03-23.657Z" fill="url(#prize-3_svg__o)"></path>
          <path d="m99.904 168.502-21.03-23.657h42.06l-21.03 23.657Z" fill="url(#prize-3_svg__p)"></path>
          <g filter="url(#prize-3_svg__q)">
            <path
              d="m99.329 39.559 2.436 7.12 7.409 2.342-7.409 2.342-2.436 7.12-2.436-7.12-7.409-2.342 7.409-2.342 2.436-7.12Z"
              fill="#fff"
              fill-opacity="0.62"
            ></path>
            <path
              d="m99.329 39.787 2.366 6.916.012.036.036.011 7.185 2.271-7.185 2.271-.036.012-.012.035-2.366 6.916-2.366-6.916-.012-.035-.036-.012-7.185-2.27 7.185-2.272.036-.011.012-.036 2.366-6.916Z"
              stroke="#FFC886"
              stroke-width="0.148"
            ></path>
          </g>
          <path d="m160.718 134.753-31.83 5.678 21.03-35.012 10.8 29.334Z" fill="url(#prize-3_svg__r)"></path>
          <path d="m39.087 67.25 31.83-5.677-21.03 35.012-10.8-29.334Z" fill="url(#prize-3_svg__s)"></path>
          <path d="m160.72 67.253-10.799 29.334-21.03-35.011 31.829 5.677Z" fill="url(#prize-3_svg__t)"></path>
          <path d="m39.093 134.751 10.799-29.335 21.03 35.012-31.83-5.677Z" fill="url(#prize-3_svg__u)"></path>
          <path
            d="M154.014 100.368c0 28.351-23.915 51.359-53.447 51.359-29.531 0-53.447-23.008-53.447-51.359 0-28.351 23.916-51.359 53.447-51.359 29.532 0 53.447 23.008 53.447 51.359Z"
            fill="url(#prize-3_svg__v)"
            stroke="url(#prize-3_svg__w)"
            stroke-width="0.741"
          ></path>
          <g filter="url(#prize-3_svg__x)">
            <ellipse cx="100.559" cy="100.373" rx="47.254" ry="45.421" fill="url(#prize-3_svg__y)"></ellipse>
          </g>
          <g filter="url(#prize-3_svg__z)">
            <ellipse cx="100.566" cy="100.374" rx="39.379" ry="37.851" fill="url(#prize-3_svg__A)"></ellipse>
          </g>
          <path
            d="M107.699 99.717c2.008.783 3.557 1.924 4.646 3.422 1.09 1.498 1.634 3.336 1.634 5.515 0 2.314-.612 4.306-1.838 5.974-1.191 1.668-2.825 2.928-4.902 3.779s-4.392 1.276-6.945 1.276c-3.268 0-6.06-.732-8.374-2.195-2.281-1.498-3.915-3.677-4.902-6.537l6.842-3.983c.477 1.634 1.277 2.877 2.4 3.728a6.104 6.104 0 0 0 3.779 1.277c1.362 0 2.485-.358 3.37-1.073.919-.749 1.379-1.77 1.379-3.063 0-2.894-2.417-4.341-7.251-4.341H96.26v-7.047h2.094c1.634 0 2.911-.391 3.83-1.174.953-.817 1.429-1.822 1.429-3.013 0-1.09-.374-1.957-1.123-2.604-.749-.681-1.702-1.022-2.86-1.022-1.293 0-2.434.443-3.42 1.328-.988.885-1.72 2.128-2.197 3.728l-6.536-3.779c.885-2.927 2.468-5.157 4.75-6.69 2.314-1.565 5.054-2.348 8.22-2.348 2.418 0 4.562.442 6.435 1.328 1.906.885 3.37 2.127 4.391 3.727 1.055 1.6 1.583 3.438 1.583 5.515 0 1.906-.443 3.575-1.328 5.004-.885 1.396-2.161 2.485-3.829 3.268ZM79.563 67.564l.974 2.849 2.964.937-2.964.936-.974 2.849-.975-2.849-2.963-.936 2.963-.937.975-2.849ZM67.743 54.952l2.274 6.646 6.914 2.186-6.914 2.186-2.274 6.646-2.274-6.646-6.914-2.186 6.914-2.186 2.274-6.646Z"
            fill="#fff"
          ></path>
          <defs>
            <filter
              id="prize-3_svg__a"
              x="7.846"
              y="105.854"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.11 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5620_22965"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__b"
              x="-5.717"
              y="91.614"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.19 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5620_22965"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__c"
              x="-18.912"
              y="73.306"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.42 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5620_22965"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__d"
              x="71.674"
              y="105.854"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.11 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5620_22965"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__e"
              x="85.237"
              y="91.614"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.19 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5620_22965"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__f"
              x="98.432"
              y="73.306"
              width="119.238"
              height="75.438"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="23.881"></feOffset>
              <feGaussianBlur stdDeviation="11.94"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-23.881" dy="-47.761"></feOffset>
              <feGaussianBlur stdDeviation="2.985"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.42 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5620_22965"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__g"
              x="31.926"
              y="31.573"
              width="136.163"
              height="115.58"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="23.881"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__i"
              x="57.52"
              y="36.212"
              width="115.843"
              height="135.638"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="23.881"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__k"
              x="32.02"
              y="60.998"
              width="136.163"
              height="115.58"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="23.881"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__m"
              x="26.747"
              y="36.303"
              width="115.843"
              height="115.577"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="23.881"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5620_22965"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5620_22965" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__q"
              x="85.781"
              y="35.855"
              width="27.095"
              height="26.334"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feGaussianBlur stdDeviation="1.852" result="effect1_foregroundBlur_5620_22965"></feGaussianBlur>
            </filter>
            <filter
              id="prize-3_svg__x"
              x="53.305"
              y="53.471"
              width="94.508"
              height="92.323"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="-1.482"></feOffset>
              <feGaussianBlur stdDeviation="1.482"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0.172667 0 0 0 0 0.616667 0 0 0 0.15 0"></feColorMatrix>
              <feBlend in2="shape" result="effect1_innerShadow_5620_22965"></feBlend>
            </filter>
            <filter
              id="prize-3_svg__z"
              x="61.188"
              y="61.042"
              width="78.758"
              height="78.664"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="1.482"></feOffset>
              <feGaussianBlur stdDeviation="3.704"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0.4875 0 0 0 0 0.1755 0 0 0 0 0 0 0 0 1 0"></feColorMatrix>
              <feBlend in2="shape" result="effect1_innerShadow_5620_22965"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="-1.482"></feOffset>
              <feGaussianBlur stdDeviation="3.704"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 1 0 0 0 0 0.716167 0 0 0 0 0.454167 0 0 0 1 0"></feColorMatrix>
              <feBlend in2="effect1_innerShadow_5620_22965" result="effect2_innerShadow_5620_22965"></feBlend>
            </filter>
            <linearGradient
              id="prize-3_svg__o"
              x1="91.166"
              y1="42.965"
              x2="108.65"
              y2="42.965"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#FFC786"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#D18E5C"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__p"
              x1="108.646"
              y1="159.039"
              x2="91.162"
              y2="159.039"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#FFC786"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#D18E5C"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__r"
              x1="156.563"
              y1="122.745"
              x2="148.329"
              y2="137.581"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#FFC786"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#D18E5C"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__s"
              x1="43.242"
              y1="79.259"
              x2="51.475"
              y2="64.423"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#FFC786"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#D18E5C"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__t"
              x1="147.823"
              y1="64.707"
              x2="156.057"
              y2="79.544"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#FFC786"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#D18E5C"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__u"
              x1="51.989"
              y1="137.296"
              x2="43.756"
              y2="122.46"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.489" stop-color="#FFC786"></stop>
              <stop offset="0.489" stop-color="#D1E5EE"></stop>
              <stop offset="0.489" stop-color="#D18E5C"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__v"
              x1="66.069"
              y1="61.903"
              x2="134.692"
              y2="141.533"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#FFC887"></stop>
              <stop offset="0.521" stop-color="#FFE7CB"></stop>
              <stop offset="1" stop-color="#B45612"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__w"
              x1="100.567"
              y1="48.639"
              x2="100.567"
              y2="152.097"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#fff" stop-opacity="0.5"></stop>
              <stop offset="1" stop-color="#fff" stop-opacity="0"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__y"
              x1="70.369"
              y1="65.677"
              x2="127.939"
              y2="137.939"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#D28E5D"></stop>
              <stop offset="1" stop-color="#FFC887"></stop>
            </linearGradient>
            <linearGradient
              id="prize-3_svg__A"
              x1="74.507"
              y1="69.203"
              x2="104.86"
              y2="139.126"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#FFCD92"></stop>
              <stop offset="0.484" stop-color="#D88335"></stop>
              <stop offset="1" stop-color="#9C5A2A"></stop>
            </linearGradient>
          </defs>
        </svg>
        <span
          v-else
          class="h-[24px] self-start px-[16px] ltr:right-0 rtl:left-0 top-0 bg-[#08FFFF] text-[#000] rounded-[4px]"
        >
          {{ index + 1 }}
        </span>
      </div>
      <div class="flex gap-[24px] leading-4 mb-3">
        <div class="max-w-[50%] flex-1">
          <div
            class="text-[#08FFFF] text-[16px] leading-[22px] font-bold md:text-[20px] lg:text-[24px] lg:leading-[30px] kcgi_alternate__PfGS3"
          >
            {{ volume }}
          </div>
          <span class="text-[#fff] text-[12px] leading-[16px] lg:text-[14px] lg:leading-[20px]"
            >Trading volume (USDT)</span
          >
        </div>
        <div class="max-w-[50%] flex-1">
          <div
            class="text-[#08FFFF] text-[16px] leading-[22px] font-bold md:text-[20px] lg:text-[24px] lg:leading-[30px] kcgi_alternate__PfGS3"
          >
            {{ amount }}
          </div>
          <span class="text-[#fff] text-[12px] leading-[16px] lg:text-[14px] lg:leading-[20px]">Rewards (USDT)</span>
        </div>
      </div>
    </div>
  </div>
  <!-- <div
    class="overflow-hidden relative mb-[12px] md:mb-[24px] flex py-[12px] px-[16px] md:py-[20px] lg:py-[28px] xl:py-[32px] border-[#00FFF1] border-[0.5px] md:border-1 border-solid rounded-[8px] md:rounded-[16px]"
  >
    <div class="flex flex-1 w-0">
      <img
        src="https://img.bitgetimg.com/multiLang/web/a7992caa12815a8decffe0584899ba33.png"
        class="border-[1px] border-solid border-[#fff] block w-[24px] h-[24px] rounded-[99px] ltr:mr-[8px] rtl:ml-[8px] md:w-[48px] md:h-[48px] md:ltr:mr-[12px] md:rtl:ml-[12px] lg:w-[64px] lg:h-[64px] xl:w-[80px] xl:h-[80px] xl:ltr:mr-[20px] xl:rtl:ml-[20px]"
        alt=""
      />
      <div
        class="flex items-center truncate text-[#fff] text-[16px] leading-[24px] mb-[12px] w-[70%] md:text-[20px] md:leading-[22px] lg:text-[16px] lg:leading-[24px] lg:mb-[16px] xl:text-[20px] xl:leading-[24px] lg:mb-[24px]"
      >
        <span class="border-[0px] cursor-pointer inline-block">CryptoSquad</span>
        <svg
          width="1em"
          height="1em"
          viewBox="0 0 280 272"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="w-[48px] h-[48px] ml-auto"
        >
          <g filter="url(#prize-1_svg__a)">
            <path
              d="M44.46 149.438c-.597-3.926 2.748-7.335 6.687-6.816l88.177 11.621a5.937 5.937 0 0 1 5.139 6.416l-1.406 15.814a5.98 5.98 0 0 1-6.751 5.392l-84.33-11.39a5.935 5.935 0 0 1-5.078-4.991l-2.439-16.046Z"
              fill="#FF7B01"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__b)">
            <path
              d="M25.467 129.193c-.596-3.925 2.748-7.335 6.687-6.815l88.177 11.621a5.937 5.937 0 0 1 5.14 6.416l-1.407 15.814a5.978 5.978 0 0 1-6.75 5.392l-84.331-11.39a5.935 5.935 0 0 1-5.077-4.992l-2.439-16.046Z"
              fill="#FFA001"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__c)">
            <path
              d="M6.999 103.169c-.597-3.926 2.748-7.335 6.687-6.816l88.177 11.622a5.937 5.937 0 0 1 5.14 6.415l-1.407 15.815a5.978 5.978 0 0 1-6.75 5.391l-84.332-11.39a5.935 5.935 0 0 1-5.077-4.991L7 103.169Z"
              fill="#FECC50"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__d)">
            <path
              d="M233.798 149.451c.597-3.926-2.748-7.335-6.687-6.816l-88.177 11.622a5.937 5.937 0 0 0-5.14 6.416l1.407 15.814a5.979 5.979 0 0 0 6.75 5.392l84.332-11.39a5.937 5.937 0 0 0 5.076-4.992l2.439-16.046Z"
              fill="#FF7B01"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__e)">
            <path
              d="M252.783 129.193c.596-3.925-2.748-7.335-6.687-6.815l-88.177 11.621a5.937 5.937 0 0 0-5.14 6.416l1.407 15.814a5.978 5.978 0 0 0 6.75 5.392l84.331-11.39a5.935 5.935 0 0 0 5.077-4.992l2.439-16.046Z"
              fill="#FFA001"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__f)">
            <path
              d="M271.251 103.169c.597-3.926-2.748-7.335-6.687-6.816l-88.177 11.622a5.937 5.937 0 0 0-5.14 6.415l1.407 15.815a5.978 5.978 0 0 0 6.751 5.391l84.331-11.39a5.937 5.937 0 0 0 5.077-4.991l2.438-16.046Z"
              fill="#FECC50"
            ></path>
          </g>
          <g filter="url(#prize-1_svg__g)">
            <mask
              id="prize-1_svg__h"
              maskUnits="userSpaceOnUse"
              x="111"
              y="76"
              width="58"
              height="58"
              style="mask-type: alpha"
            >
              <path
                d="M128.285 81.23c6.505-6.396 16.937-6.396 23.442 0l6.161 6.06 5.762 5.666c6.661 6.55 6.661 17.287 0 23.837l-5.762 5.667-6.161 6.058c-6.505 6.397-16.937 6.397-23.442 0l-6.161-6.058-5.762-5.667c-6.66-6.55-6.66-17.287 0-23.837l5.762-5.667 6.161-6.059Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-1_svg__h)" fill="#FFD0F5">
              <path d="m211.533 140.045-35.764-35.171-35.764 35.171h71.528Z"></path>
              <path d="M68.477 140.045h71.528l-35.764-35.171-35.764 35.171Z"></path>
            </g>
          </g>
          <g filter="url(#prize-1_svg__i)">
            <mask
              id="prize-1_svg__j"
              maskUnits="userSpaceOnUse"
              x="147"
              y="111"
              width="58"
              height="58"
              style="mask-type: alpha"
            >
              <path
                d="M199.481 128.058c6.661 6.55 6.661 17.288 0 23.838l-5.762 5.666-6.161 6.059c-6.504 6.397-16.937 6.397-23.442 0l-6.161-6.059-5.762-5.666c-6.66-6.55-6.66-17.288 0-23.838l5.762-5.666 6.161-6.059c6.505-6.397 16.938-6.397 23.442 0l6.161 6.059 5.762 5.666Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-1_svg__j)" fill="#FFD0F5">
              <path d="m140.073 210.313 35.764-35.17-35.764-35.171v70.341Z"></path>
              <path d="M140.073 69.632v70.34l35.764-35.17-35.764-35.17Z"></path>
            </g>
          </g>
          <g filter="url(#prize-1_svg__k)">
            <mask
              id="prize-1_svg__l"
              maskUnits="userSpaceOnUse"
              x="111"
              y="146"
              width="58"
              height="58"
              style="mask-type: alpha"
            >
              <path
                d="M151.863 198.853c-6.505 6.396-16.937 6.396-23.442 0l-6.161-6.059-5.762-5.667c-6.661-6.55-6.661-17.287 0-23.837l5.762-5.667 6.161-6.058c6.505-6.397 16.937-6.397 23.442 0l6.161 6.058 5.762 5.667c6.661 6.55 6.661 17.287 0 23.837l-5.762 5.667-6.161 6.059Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-1_svg__l)" fill="#FFD0F5">
              <path
                d="m68.615 140.038 35.764 35.171 35.765-35.171H68.615ZM211.672 140.038h-71.528l35.764 35.171 35.764-35.171Z"
              ></path>
            </g>
          </g>
          <g filter="url(#prize-1_svg__m)">
            <mask
              id="prize-1_svg__n"
              maskUnits="userSpaceOnUse"
              x="75"
              y="111"
              width="58"
              height="58"
              style="mask-type: alpha"
            >
              <path
                d="M80.667 152.027c-6.66-6.55-6.66-17.288 0-23.838l5.762-5.666 6.161-6.059c6.505-6.397 16.937-6.397 23.442 0l6.161 6.059 5.762 5.666c6.661 6.55 6.661 17.288 0 23.838l-5.762 5.666-6.161 6.059c-6.505 6.397-16.937 6.397-23.442 0l-6.161-6.059-5.762-5.666Z"
                fill="#C4C4C4"
              ></path>
            </mask>
            <g mask="url(#prize-1_svg__n)">
              <path d="m140.075 69.772-35.764 35.17 35.764 35.171V69.772Z" fill="#FFD0F5"></path>
            </g>
          </g>
          <path d="m138.354 42.226 28.994 33.119H109.36l28.994-33.12Z" fill="url(#prize-1_svg__o)"></path>
          <path d="m138.357 231.226-28.994-33.12h57.988l-28.994 33.12Z" fill="url(#prize-1_svg__p)"></path>
          <g filter="url(#prize-1_svg__q)">
            <path
              d="m138.362 51.065 3.359 9.969 10.213 3.278-10.213 3.279-3.359 9.969-3.359-9.97-10.214-3.278 10.214-3.278 3.359-9.97Z"
              fill="#fff"
            ></path>
            <path
              d="m138.362 51.39 3.26 9.677.017.05.05.015 9.906 3.18-9.906 3.18-.05.016-.017.05-3.26 9.677-3.261-9.677-.017-.05-.05-.016-9.906-3.18 9.906-3.18.05-.016.017-.05 3.261-9.677Z"
              stroke="#FAFF00"
              stroke-width="0.207"
            ></path>
          </g>
          <path d="m222.198 183.977-43.883 7.949 28.994-49.016 14.889 41.067Z" fill="url(#prize-1_svg__r)"></path>
          <path d="m54.505 89.474 43.883-7.949-28.994 49.017-14.889-41.068Z" fill="url(#prize-1_svg__s)"></path>
          <path d="m222.201 89.478-14.889 41.067-28.994-49.016 43.883 7.949Z" fill="url(#prize-1_svg__t)"></path>
          <path d="M54.51 183.974 69.4 142.906l28.994 49.016-43.883-7.948Z" fill="url(#prize-1_svg__u)"></path>
          <path
            d="M212.938 135.849c0 39.699-32.975 71.902-73.678 71.902-40.704 0-73.679-32.203-73.679-71.902 0-39.7 32.975-71.903 73.679-71.903 40.703 0 73.678 32.204 73.678 71.903Z"
            fill="url(#prize-1_svg__v)"
            stroke="url(#prize-1_svg__w)"
            stroke-width="1.037"
          ></path>
          <g filter="url(#prize-1_svg__x)">
            <ellipse cx="139.25" cy="135.841" rx="65.149" ry="63.589" fill="url(#prize-1_svg__y)"></ellipse>
          </g>
          <g filter="url(#prize-1_svg__z)">
            <ellipse cx="139.259" cy="135.846" rx="54.291" ry="52.991" fill="url(#prize-1_svg__A)"></ellipse>
          </g>
          <path
            d="M122.472 129.05v-11.439l16.371-9.15h9.579v52.401h-12.367v-39.319l-13.583 7.507ZM110.304 89.913l1.344 3.988 4.085 1.311-4.085 1.312-1.344 3.987-1.344-3.987-4.085-1.312 4.085-1.311 1.344-3.988ZM94.02 72.252l3.135 9.304 9.532 3.06-9.532 3.06-3.136 9.305-3.135-9.304-9.532-3.06 9.532-3.06 3.135-9.305Z"
            fill="#fff"
          ></path>
          <defs>
            <filter
              id="prize-1_svg__a"
              x="10.958"
              y="142.569"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.11 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__b"
              x="-8.034"
              y="122.325"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.19 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__c"
              x="-26.503"
              y="96.301"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.42 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__d"
              x="100.341"
              y="142.583"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.11 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__e"
              x="119.325"
              y="122.325"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.19 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__f"
              x="137.794"
              y="96.301"
              width="166.959"
              height="106.215"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="33.433"></feOffset>
              <feGaussianBlur stdDeviation="16.716"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dx="-33.433" dy="-66.866"></feOffset>
              <feGaussianBlur stdDeviation="4.179"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.42 0"></feColorMatrix>
              <feBlend mode="overlay" in2="shape" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__g"
              x="44.502"
              y="38.008"
              width="191.012"
              height="162.174"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="33.433"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__i"
              x="80.33"
              y="44.67"
              width="162.372"
              height="190.615"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="33.433"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__k"
              x="44.634"
              y="79.901"
              width="191.012"
              height="162.174"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="33.433"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__m"
              x="37.447"
              y="44.8"
              width="162.372"
              height="162.177"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset></feOffset>
              <feGaussianBlur stdDeviation="33.433"></feGaussianBlur>
              <feColorMatrix values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0"></feColorMatrix>
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow_5589_132916"></feBlend>
              <feBlend in="SourceGraphic" in2="effect1_dropShadow_5589_132916" result="shape"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__q"
              x="121.678"
              y="47.953"
              width="33.371"
              height="32.718"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feGaussianBlur stdDeviation="1.556" result="effect1_foregroundBlur_5589_132916"></feGaussianBlur>
            </filter>
            <filter
              id="prize-1_svg__x"
              x="74.102"
              y="70.178"
              width="130.297"
              height="129.253"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="-2.074"></feOffset>
              <feGaussianBlur stdDeviation="1.037"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0.616667 0 0 0 0 0.407 0 0 0 0 0 0 0 0 0.25 0"></feColorMatrix>
              <feBlend in2="shape" result="effect1_innerShadow_5589_132916"></feBlend>
            </filter>
            <filter
              id="prize-1_svg__z"
              x="84.969"
              y="80.781"
              width="108.578"
              height="110.131"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
              <feBlend in="SourceGraphic" in2="BackgroundImageFix" result="shape"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="2.074"></feOffset>
              <feGaussianBlur stdDeviation="2.074"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 0.7 0 0 0 0 0.465967 0 0 0 0 0.0116667 0 0 0 1 0"></feColorMatrix>
              <feBlend in2="shape" result="effect1_innerShadow_5589_132916"></feBlend>
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              ></feColorMatrix>
              <feOffset dy="-2.074"></feOffset>
              <feGaussianBlur stdDeviation="1.037"></feGaussianBlur>
              <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"></feComposite>
              <feColorMatrix values="0 0 0 0 1 0 0 0 0 0.72 0 0 0 0 0 0 0 0 1 0"></feColorMatrix>
              <feBlend in2="effect1_innerShadow_5589_132916" result="effect2_innerShadow_5589_132916"></feBlend>
            </filter>
            <linearGradient
              id="prize-1_svg__o"
              x1="126.302"
              y1="55.473"
              x2="150.407"
              y2="55.473"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__p"
              x1="150.409"
              y1="217.978"
              x2="126.304"
              y2="217.978"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__r"
              x1="216.47"
              y1="167.166"
              x2="204.85"
              y2="187.785"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__s"
              x1="60.233"
              y1="106.285"
              x2="71.853"
              y2="85.666"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__t"
              x1="204.42"
              y1="85.913"
              x2="216.04"
              y2="106.533"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__u"
              x1="72.291"
              y1="187.538"
              x2="60.671"
              y2="166.918"
              gradientUnits="userSpaceOnUse"
            >
              <stop offset="0.485" stop-color="#FFE590"></stop>
              <stop offset="0.489" stop-color="#FFC700"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__v"
              x1="91.697"
              y1="81.997"
              x2="187.977"
              y2="192.019"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#FFECA9"></stop>
              <stop offset="0.237" stop-color="#FFD600"></stop>
              <stop offset="1" stop-color="#F90"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__w"
              x1="139.26"
              y1="63.428"
              x2="139.26"
              y2="208.27"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#fff" stop-opacity="0.5"></stop>
              <stop offset="1" stop-color="#fff" stop-opacity="0"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__y"
              x1="97.627"
              y1="87.266"
              x2="178.493"
              y2="187.225"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#FFC700"></stop>
              <stop offset="1" stop-color="#D58500"></stop>
            </linearGradient>
            <linearGradient
              id="prize-1_svg__A"
              x1="103.332"
              y1="92.207"
              x2="146.271"
              y2="189.618"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#FFB13C"></stop>
              <stop offset="0.484" stop-color="#B45F1D"></stop>
              <stop offset="1" stop-color="#743110"></stop>
            </linearGradient>
          </defs>
        </svg>
      </div>
      <div class="flex gap-[24px]">
        <div class="max-w-[50%] flex-1">
          <div
            class="text-[#08FFFF] text-[16px] leading-[22px] font-bold md:text-[20px] lg:text-[24px] lg:leading-[30px] kcgi_alternate__PfGS3"
          >
            15,045,110.75
          </div>
          <span class="text-[#fff] text-[12px] leading-[16px] lg:text-[14px] lg:leading-[20px]"
            >Trading volume (USDT)</span
          >
        </div>
        <div class="max-w-[50%] flex-1">
          <div
            class="text-[#08FFFF] text-[16px] leading-[22px] font-bold md:text-[20px] lg:text-[24px] lg:leading-[30px] kcgi_alternate__PfGS3"
          >
            10,623.66
          </div>
          <span class="text-[#fff] text-[12px] leading-[16px] lg:text-[14px] lg:leading-[20px]">Rewards (USDT)</span>
        </div>
      </div>
    </div>
  </div> -->
</template>
