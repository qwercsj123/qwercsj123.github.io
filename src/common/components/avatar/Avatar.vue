<template>
  <div class="avatar">
    <div class="avatar-bg">
      <a-avatar :src="src" :size="170" class="avatar-img" />
    </div>
    <div class="avatar-name">{{ name }}</div>
  </div>
</template>

<script setup>
const props = defineProps({
  src: {
    type: String,
    default: '',
  },
  name: {
    type: String,
    default: '',
  },
});
</script>

<style scoped lang="less">
.avatar {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;

  .avatar-bg {
    width: 235px;
    height: 221px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: url("../../../assets/circle.png");
    background-size: 100% 100%;
    position: relative;

    .avatar-img {
      position: absolute;
      top: 11px;
    }
  }

  .avatar-name {
    color: #C99932;
    font-family: HarmonyOS_Sans_SC_Black;
    text-align: center;
    font-style: normal;
    text-transform: none;
    font-size: 24px;
    font-weight: bold;
    text-align: center;
  }
}
</style>
