<template>
  <div class="container" :style="{
    background: bg
  }">
    <div class="content">
      <slot></slot>
    </div>
  </div>
</template>

<script setup>
import { computed } from 'vue';
import { defineProps } from 'vue';

const props = defineProps({
  mode: {
    type: String,
    default: 'light',
    validator: (value) => ['dark', 'light'].includes(value),
  },
});
const bg = computed(() => props.mode === 'dark' ? '#EDEDED' : '#fff')
</script>

<style scoped lang="less">
.container {
  display: flex;
  justify-content: center;

  .content {
    width: 1212px;
  }
}

  @media only screen and(min-width: 10px) and (max-width: 850px)  {

  // 在这个宽度范围内执行某个操作
  .content {
    width: 100% !important;
  }
}
</style>
