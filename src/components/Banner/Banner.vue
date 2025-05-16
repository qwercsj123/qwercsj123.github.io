<template>
  <div class="banner-container">
    <div class="banner">
      <div class="title-container">
        Advancing Data for Better Health:<br> Reliable LLM Application in People-Centric Healthcare
      </div>
    </div>
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
  aspect-ratio: 1280 / 243;
  background-image: url("../../assets/bannerPlus.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.title-container{
  color: white;
  font-family: Montserrat, "Helvetica Neue", Helvetica, Arial, sans-serif;
  text-transform: uppercase;
  font-weight: 700;
  font-size: 40px;
  line-height: 60px;
  margin-bottom: 20px;
  padding-top: 40px;
  padding-left: 50px;
}

@media only screen and(max-width: 960px) {
  .banner-container {
    padding-top: 54px !important;
  }

  .banner {
    aspect-ratio: 750 / 315;
    background-image: url("../../assets/banner_m.png");
    background-size: cover;
    background-position: center;
  }
  .title-container{
    padding-top: -30px;
    color: white;
    font-family: Montserrat, "Helvetica Neue", Helvetica, Arial, sans-serif;
    text-transform: uppercase;
    font-weight: 720;
    font-size: 15px;
    line-height: 20px;
    margin-bottom: 20px;
  }
}
</style>
