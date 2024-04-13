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
  { id: 1, name: 'Shenda Hong', img: shen, content: 'Shenda Hong(hongshenda@pku.edu.cn) is an Assistant Professor (tenure-track) in National Institute of Health Data Science (NIHDS) at Peking University. His research interests are health data science and artificial intelligence for real-world healthcare data, especially for temporal medical data. He serves as an associate editor of Health Data Science; a program committee member or reviewer for international conferences including KDD, ICLR, NeurIPS, ICML, AAAI and IJCAI; an external reviewer of Center for Medical Device Evaluation (National Medical Products Administration, NMPA) of China.' },
  { id: 2, name: 'Tianfan Fu', img: fu, content: 'Tianfan Fu(futianfan@gmail.com) is a tenure-track assistant professor at Rensselaer Polytechnic Institute (RPI) Computer Science Department. He obtained Ph.D. degree from the Department of Computational Science and Engineering at Georgia Institute of Technology in 2023, supervised by Prof. Jimeng Sun. His research interests span a wide range of areas within artificial intelligence, with a focus on applications in drug discovery, science (biology/chemistry/pharma), drug development (clinical trial), and healthcare.' },
  { id: 3, name: 'Liantao Ma', img: ma, content: 'Liantao Ma(malt@pku.edu.cn) is a Research Assistant Professor at the National Engineering Research Center for Software Engineering at Peking University. He graduated with a Ph.D. at Peking University, where he also completed his postdoctoral training. His main research interests focus on prognosis prediction and diagnostic-therapeutic assistance based on the analysis of electronic medical record data.' },
  { id: 4, name: 'Mengling Feng', img: feng, content: 'Mengling Feng(ephfm@nus.edu.sg) is an Assistant Professor at the National University of Singapore (NUS), affiliated with the Saw Swee Hock School of Public Health (SSHSPH), School of Computer Science, and Yong Loo Lin School of Medicine. With a focus on artificial intelligence solutions for healthcare challenges. He has been involved in the construction of MIMIC-III (‘Medical Information Mart for Intensive Care’) Database.' },
  { id: 5, name: 'Capucine Van Rechem', img: van, content: 'Capucine Van Rechem(cvrechem@stanford.edu) is an Assistant Professor of Pathology at Stanford University School of Medicine. She is interested in the molecular impact of chromatin modifiers on disease development, with an emphasis on cancer. Her laboratory undertakes a cell-cycle specific angle to explore specific functions such as gene expression and replication timing. They also explore unconventional direct roles for these factors in the cytoplasm, with a focus on protein synthesis. Their ultimate goal is to provide needed insights into new targeted therapies.' },
  { id: 6, name: 'Jin Jing', img: jin, content: 'Jin Jing(jjing@mgh.harvard.edu) obtained her PhD degree in Electrical and Biomedical Engineering working in the field of signal processing and machine learning applied in clinical epilepsy from Nanyang Technological University (Singapore). She is a faculty at Harvard Medical School, a staff scientist and research instructor at Beth Israel Deaconess Medical Center, where she develops machine learning approaches to improve medical care for patients with neurological problems. %Her work establishes a unique infrastructure to bridge the worlds of clinical neurology and computational sciences by bringing together clinical and technical approaches to create new tools that solve real-world clinical problems. Her academic achievements appear in more than 50 peer-reviewed publications to date. She is the author of a best-selling book, “Atlas of Intensive Care Quantitative EEG”.' },
  { id: 7, name: 'Yuxi Zhou', img: zhou, content: 'Yuxi Zhou(joy_yuxi@pku.edu.cn) obtained the Ph.D. degree from the Key Laboratory of Machine Perception, Peking University, China, in 2021. Currently, she is a postdoctoral scholar in Beijing National Research Center for Information Science and Technology at Tsinghua University and also a lecturer in the School of Computer Science and Engineering at Tianjin University of Technology. Her main research interests include machine learning, data mining, artificial intelligence for healthcare, especially intelligent diagnosis of temporal medical data.' },

])
</script>

<style scoped lang="less">
.program {
  margin-top: 110px;
}
</style>
