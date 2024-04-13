<template>
  <div class="banner-container">
    <div class="banner"></div>
  </div>
</template>

<script setup>
</script>

<style scoped lang="less">
.banner-container {
  padding-top: 72px;
  background-color: black;
}

.banner {
  width: 100%;
  aspect-ratio: 1920 / 374;
  background-image: url("../../assets/banner.jpg");
  background-repeat: no-repeat;
  background-size: contain;
}

@media only screen and(max-width: 960px) {
  .banner-container {
    padding-top: 54px !important;
  }

  .banner {
    aspect-ratio: 750 / 315;
    background-image: url("../../assets/banner_m.jpg");

  }
}
</style>
