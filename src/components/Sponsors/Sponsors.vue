<template>
  <Page mode="dark">
    <div class="sponsors" id="Sponsors">
      <div class="c-title">Sponsors</div>
      <div class="center">
        <div class="c-paragraph c-text-center">We have confirmed sponsorship from Health Data Science, a Science Partner
          Journal. The fund will be mainly used to provide travel awards to encourage students, women, and minority
          attendees. The expected total budget is around $3,000.</div>
      </div>
    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
</script>

<style scoped lang="less">
.sponsors {
  margin-top: 110px;
  margin-bottom: 94px;

  .center {
    display: flex;
    justify-content: center;

    .c-paragraph {
      width: 980px;
    }
  }
}
</style>
