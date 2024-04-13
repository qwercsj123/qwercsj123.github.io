<template>
  <Page>
    <div class="steering" id="Organizers">
      <div class="c-title">Steering Committee</div>
      <div class="c-info-list">
        <Info v-for="info in listData" :key="info.id" :src="info.img" :name="info.name" :content="info.content"></Info>
      </div>
    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
import Info from "@/common/components/Info/Info.vue"
import fei from "@/assets/03.jpg"
import luo from "@/assets/05.jpg"
import lu from "@/assets/07.jpg"
import m from "@/assets/12.jpg"
import lucas from "@/assets/13.jpg"
import { ref } from "vue";

const listData = ref([
  { id: 1, name: 'Fei Wang', img: fei, content: '(few2001@med.cornell.edu) is a Professor of Population Health Sciences at Weill Cornell Medical College, specializing in the development of data mining and machine learning methodologies for health data science. His research interests encompass health data science, clinical risk prediction models, disease subtyping, and computational drug discovery and design. He has chaired the KDD Health Day multiple times, and has organized the KDD Workshop on Applied Data Science for Healthcare for several consecutive years.' }, 
  { id: 2, name: 'Jiebo Luo', img: luo, content: '(jluo@cs.rochester.edu) is a Professor of Computer Science at the University of Rochester. His research interests include computer vision, natural language processing, machine learning, data mining, computational social science, and digital health. He is a Fellow of ACM, AAAI, IEEE, SPIE and IAPR. He is active in the organizing or program committees of numerous technical conferences.' }, 
  { id: 3, name: 'Luxia Zhang', img: lu, content: '(zhanglx@bjmu.edu.cn) is a Professor in the renal division of Peking University First Hospital. Her research focuses on prevalence, risk factors, intervention, and management of kidney disease in China. Most of her work provides first-hand information on kidney disease in China and has gained wide attention internationally. During the last several years, her study interests have been expanded to the management of major non-communicable chronic diseases by leveraging the power of big data and machine learning.' },
  { id: 4, name: 'M. Brandon Westover', img: m, content: '(mwestover@partners.org) is an Associate Professor in Neurology at Massachusetts General Hospital (MGH) and Harvard Medical School (HMS), where he directs the MGH Critical Care EEG Monitoring Service and the MGH Clinical Data AI Center. An internationally renowned clinician scientist, physician, and technical innovator, he has created a legacy of multidisciplinary teams using engineering and AI to tackle the most pressing challenges in brain disease. His research interests lie in clinical neurophysiology, biomedical signal processing, seizures, medical decision analysis, electroencephalography, and medical informatics.' },
  { id: 5, name: 'Lucas Glass', img: lucas, content: '(lucas.glass@iqvia.com) is the global head of IQVIA’s Analytics Center of Excellence. The Center is responsible for researching, developing and operationalizing machine learning and data science solutions in the R\&D business. He started his career in pharmaceutical data science 15 years ago at Center, working on pharmacovigilance data mining algorithms. Now he is a Ph.D. candidate at Temple University, where he is researching deep learning embedding techniques on large-scale healthcare data.' },
])
</script>

<style scoped lang="less">
.steering {
  margin-top: 130px;
}
</style>
