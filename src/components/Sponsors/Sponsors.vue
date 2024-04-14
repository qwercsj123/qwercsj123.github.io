<template>
  <Page mode="dark">
    <div class="sponsors" id="Sponsors">
      <div class="c-title">Sponsors</div>
      <div class="center">
        <img class="footer-logo" :src="footerLogo" alt="">
        <div class="c-paragraph c-text-center">Sponsored by <span style="font-weight: bold;font-style: italic;">Health Data Science</span>, a Science Partner Journal.</div>
      </div>
    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
import footerLogo from "@/assets/footerLogo.png"
</script>

<style scoped lang="less">
.sponsors {
  margin-top: 110px;
  margin-bottom: 94px;

  .center {
    display: flex;
    justify-content: center;
    align-items: center;

    .footer-logo {
      width: 100px;
      height: 100px;
    }

    .c-paragraph {
      width: 980px;
      margin: 0;
    }
  }
}
</style>
