<template>
  <Page>
    <div class="program" id="Organizers">
      <div class="c-title">Program Committee</div>
<!--      <div id="organizer-wrap">-->
<!--        <iframe class="airtable-embed" src="https://airtable.com/embed/appPDKpS4OBqbgsrS/shrCrCrlRwwBaV7DG" frameborder="0" onmousewheel="" width="100%" height="750" style="background: transparent; border: 1px solid #ccc;"></iframe>-->
<!--    </div>-->
      <div class="c-info-list" style="margin-top: 80px">
        <Info v-for="info in listData" :key="info.id" :src="info.img" :name="info.name" :content="info.content"></Info>
      </div>
    </div>
  </Page>
</template>

<script setup>
import { ref } from 'vue'
import Info from "@/common/components/Info/Info.vue"
import Page from "../Page/Page.vue"
import feng from "@/assets/22.jpg"
import van from "@/assets/23.jpg"
import jin from "@/assets/24.jpg"
import zhou from "@/assets/28.jpg"
import shen from "@/assets/16.jpg"
import fu from "@/assets/17.jpg"
import ma from "@/assets/18.jpg"
import pan from "@/assets/42.jpg"
import chen from "@/assets/43.jpg"
import cui from "@/assets/40.jpg"
import gao from "@/assets/41.jpg"

const listData = ref([
  { id: 1, name: 'Shenda Hong', img: shen, content: 'Shenda Hong is a tenure-track Assistant Professor in National Institute of Health Data Science (NIHDS) at Peking University. His research interests are health data science and artificial intelligence for real-world healthcare data, especially for temporal medical data. ' },
  { id: 2, name: 'Tianfan Fu', img: fu, content: 'Tianfan Fu is a tenure-track Assistant Professor at Rensselaer Polytechnic Institute (RPI) Computer Science Department. His research interests span a wide range of areas within artificial intelligence, with a focus on applications in drug discovery, science (biology/chemistry/pharma), drug development (clinical trial), and healthcare.' },
  { id: 3, name: 'Liantao Ma', img: ma, content: 'Liantao Ma is a Research Assistant Professor at the National Engineering Research Center for Software Engineering at Peking University. His main research interests focus on prognosis prediction and diagnostic-therapeutic assistance based on the analysis of electronic medical record data. ' },
  { id: 4, name: 'Mengling Feng', img: feng, content: 'Mengling Feng is an Associate Professor at the National University of Singapore (NUS), affiliated with the Saw Swee Hock School of Public Health (SSHSPH), School of Computer Science, and Yong Loo Lin School of Medicine. With a focus on artificial intelligence solutions for healthcare challenges. ' },
  { id: 5, name: 'Chengwei Pan', img: pan, content: 'Chengwei Pan is an Associate Professor at Beihang University, has been selected for the Beihang Young Talent Program. His research focuses on computer vision, computer graphics, and large language models, with specific interests in medical image analysis and processing, novel view synthesis, and security of large language models.' },
  { id: 6, name: 'Jintai Chen', img: chen, content: 'Jintai Chen is a tenure-track Assistant Professor at the Hong Kong University of Science and Technology’s Guangzhou campus. His research centers on the intersection of AI and healthcare, with a particular focus on developing generalizable and reliable foundation models to address real-world medical challenges.' },
  { id: 7, name: 'Hejie Cui', img: cui, content: 'Hejie Cui is a postdoctoral researcher at the Stanford Center for Biomedical Informatics Research at Stanford University. Her research focuses on Large Language Model (LLM) Evaluation and Post-training for Healthcarethe ,intersection of machine learning, data mining, and biomedical informatics.' },
  { id: 8, name: 'Junyi Gao', img: gao, content: 'Junyi Gao, Ph.D. student in the Health Data Research UK (HDRUK) program at the University of Edinburgh. His research focuses on AI for healthcare, including medical foundation models, individual-level healthcare modeling using EHR data, population-level epidemiological modeling, and the development of open-source healthcare toolkits for Python and R.' },

])
</script>

<style scoped lang="less">
.program {
  margin-top: 110px;
}
#organizer-wrap{
  width: 100%;
  height: 750px;
  padding: 0;
  overflow: hidden;
}
#organizer-frame{
  width: 107%; height: 750px; background: transparent; border: 1px solid #ccc;
  -ms-zoom: 0.93;
  -moz-transform: scale(0.93);
  -moz-transform-origin: 0 0;
  -o-transform: scale(0.93);
  -o-transform-origin: 0 0;
  -webkit-transform: scale(0.93);
  -webkit-transform-origin: 0 0;
}
</style>
