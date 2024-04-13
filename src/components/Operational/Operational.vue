<template>
  <Page>
    <div class="operational">
      <div class="c-title">Operational Committee</div>
      <div class="c-info-list">
        <Info v-for="info in listData" :key="info.id" :src="info.img" :name="info.name" :content="info.content"></Info>
      </div>
    </div>
  </Page>
</template>

<script setup>
import { ref } from 'vue'
import Info from "@/common/components/Info/Info.vue"
import Page from "../Page/Page.vue"
import yin from "@/assets/30.jpg"
import wang from "@/assets/31.jpg"
import yang from "@/assets/32.jpg"
import tang from "@/assets/36.jpg"
import gao from "@/assets/37.jpg"
import sun from "@/assets/38.jpg"
const listData = ref([
  { id: 1, name: 'Daoxin Yin', img: yin, content: 'Daoxin Yin, the Executive Editor for Health Data Science (HDS) and previously served as the China Editor for BMJ.' },
  { id: 2, name: 'Mai Wang', img: wang, content: 'Mai Wang, the Director of the Health Data Science (HDS) Editorial Office and the Head of the Comprehensive Department at National Institute of Health Data Science at Peking University.' },
  { id: 3, name: 'Yu Yang', img: yang, content: 'Yu Yang, Assistant Research Professor at National Institute of Health Data Science at Peking University.' },
  { id: 4, name: 'Gongzheng Tang', img: tang, content: 'Gongzheng Tang, PhD student in health data science at Peking University.' },
  { id: 5, name: 'Junyi Gao', img: gao, content: 'Junyi Gao, Ph.D. student in the Health Data Research UK (HDRUK) program at the University of Edinburgh.' },
  { id: 6, name: 'Chenxi Sun', img: sun, content: 'Chenxi Sun, PhD student in intelligence science and technology at Peking University.' },

])
</script>

<style scoped lang="less">
.operational {
  margin-top: 110px;
  margin-bottom: 150px;
}
</style>
