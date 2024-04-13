<template>
  <div class="info">
    <Avatar :src="src" :name="name"></Avatar>
    <div class="info-detail">{{ content }}</div>
  </div>
</template>

<script setup>
import Avatar from "../avatar/Avatar.vue"
const props = defineProps({
  src: {
    type: String,
    default: '',
  },
  name: {
    type: String,
    default: '',
  },
  content: {
    type: String,
    default: '',
  },
});
</script>

<style scoped lang="less">
.info {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  .info-detail {
    margin-top: 20px;
    font-family: "TimesNewRomanPSMT", sans-serif;
    font-size: 20px;
    color: #2C2F31;
    line-height: 1.8;
    text-align: justifyLeft;
    font-style: normal;
    text-transform: none;
    padding: 0 16px;
  }

}
</style>
