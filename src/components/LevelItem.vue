<script setup lang="ts">
import V2 from "../assets/v2.png";
import V3 from "../assets/v3.png";
import V5 from "../assets/v5.png";
import V6 from "../assets/v0.png";
import OfflineIcon from "../assets/offline.png";
import { computed } from "vue";

/**
 * 等级小组件
 * 注意事项:
 * 1.
 */

// 属性定义
const props = withDefaults(
  defineProps<{
    offline: boolean;
    level: number;
  }>(),
  {
    level: 5,
    offline: false,
  }
);

const levelIcon = computed(() => {
  switch (props.level) {
    case 5:
      return V5;
    case 6:
      return V6;
    case 4:
      return V3;
    case 3:
      return V3;
    case 2:
      return V2;
    default:
      return V2;
  }
});
</script>

<template>
  <span class="gap-1 flex">
    <img class="h-5 w-5" :src="levelIcon" alt="level_icon" />
    <img class="h-5 w-5" :src="OfflineIcon" v-show="offline" alt="offline_icon" />
  </span>
</template>
