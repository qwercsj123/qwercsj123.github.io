<template>
  <Page>
    <div class="program">
      <div class="c-title">Program Committee</div>
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
import feng from "@/assets/22.jpg"
import van from "@/assets/23.jpg"
import jin from "@/assets/24.jpg"
import zhou from "@/assets/28.jpg"
import shen from "@/assets/16.jpg"
import fu from "@/assets/17.jpg"
import ma from "@/assets/18.jpg"
const listData = ref([
  { id: 1, name: 'Shenda Hong', img: shen, content: 'Shenda Hong is an Assistant Professor (tenure-track) in National Institute of Health Data Science (NIHDS) at Peking University. His research interests are health data science and artificial intelligence for real-world healthcare data, especially for temporal medical data.' },
  { id: 2, name: 'Tianfan Fu', img: fu, content: 'Tianfan Fu is a tenure-track assistant professor at Rensselaer Polytechnic Institute (RPI) Computer Science Department. His research interests span a wide range of areas within artificial intelligence, with a focus on applications in drug discovery, science (biology/chemistry/pharma), drug development (clinical trial), and healthcare.' },
  { id: 3, name: 'Liantao Ma', img: ma, content: 'Liantao Ma is a Research Assistant Professor at the National Engineering Research Center for Software Engineering at Peking University. His main research interests focus on prognosis prediction and diagnostic-therapeutic assistance based on the analysis of electronic medical record data.' },
  { id: 4, name: 'Mengling Feng', img: feng, content: 'Mengling Feng is an Assistant Professor at the National University of Singapore (NUS), affiliated with the Saw Swee Hock School of Public Health (SSHSPH), School of Computer Science, and Yong Loo Lin School of Medicine. With a focus on artificial intelligence solutions for healthcare challenges.' },
  { id: 5, name: 'Capucine Van Rechem', img: van, content: 'Capucine Van Rechem is an Assistant Professor of Pathology at Stanford University School of Medicine. She is interested in the molecular impact of chromatin modifiers on disease development, with an emphasis on cancer.' },
  { id: 6, name: 'Jin Jing', img: jin, content: 'Jin Jing is a faculty at Harvard Medical School, a staff scientist and research instructor at Beth Israel Deaconess Medical Center, where she develops machine learning approaches to improve medical care for patients with neurological problems.' },
  { id: 7, name: 'Yuxi Zhou', img: zhou, content: 'Yuxi Zhou is a postdoctoral scholar in Beijing National Research Center for Information Science and Technology at Tsinghua University and also a lecturer in the School of Computer Science and Engineering at Tianjin University of Technology. Her main research interests include machine learning, data mining, artificial intelligence for healthcare, especially intelligent diagnosis of temporal medical data.' },

])
</script>

<style scoped lang="less">
.program {
  margin-top: 110px;
}
</style>
