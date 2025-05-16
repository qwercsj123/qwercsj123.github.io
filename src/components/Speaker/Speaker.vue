<template>
  <Page>
    <div class="speaker" id="InvitedSpeakers">
      <div class="c-title">INVITED SPEAKERS</div>
      <!-- <div class="c-paragraph c-text-center">To be announced.</div> -->
      <div class="InvitedSpeakerList" v-for="info in listData" :key="info.id">
        <Avatar style="width: 235px;" :src="info.img" :name="info.name"></Avatar>
        <div class="info-detail" style="flex: 1">
          <div class="topic" v-if="info.topic">Topic: {{ info.topic }}</div>
          <div class="abstract" v-if="info.abstract">
            <div class="abstract-title">Abstract:</div>
            <div class="abstract-content">{{ info.abstract }}</div>
          </div>
          <div class="bio">
            <span class="bio-title">Bio: </span>
            <span class="bio-content">{{ info.content }}</span>
          </div>
        </div>
      </div>
    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
import fei from "@/assets/new1.png"
import luo from "@/assets/new2.png"
import lu from "@/assets/new3.png"
import Avatar from "@/common/components/avatar/Avatar.vue"
import { ref } from "vue";

const listData = ref([
  { 
    id: 1, 
    name: 'Jimeng Sun', 
    img: fei, 
    topic: 'AI in Healthcare: From Drug Discovery to Clinical Applications',
    abstract: 'This talk will explore the transformative role of artificial intelligence in healthcare, focusing on recent advances in drug discovery and clinical applications. We will discuss how deep learning models are revolutionizing the way we approach medical research, from molecular design to patient care. The presentation will highlight real-world applications and future directions in AI-driven healthcare innovation.',
    content: 'Jimeng Sun is a Health Innovation Professor at the Computer Science Department and at Carle Illinois College of Medicine at the University of Illinois Urbana-Champaign (UIUC). Before coming to UIUC, he was an associate professor in the College of Computing at the Georgia Institute of Technology. His research focuses on artificial intelligence (AI) for healthcare, including deep learning for drug discovery, clinical trial optimization, computational phenotyping, clinical predictive modeling, treatment recommendation, and health monitoring.' 
  }, 
  { 
    id: 2, 
    name: 'Hongfang Liu', 
    img: luo, 
    topic: 'Translational AI in Medicine: Bridging Research and Clinical Practice',
    abstract: 'This presentation will discuss the critical role of translational AI in modern medicine, focusing on how artificial intelligence can bridge the gap between research discoveries and clinical applications. We will explore innovative approaches to implementing AI solutions in healthcare settings, addressing both technical challenges and practical considerations for successful deployment.',
    content: 'Hongfang Liu is a Professor at McWilliams School of Biomedical Informatics. She leads the research in the Center for Translational AI Excellence and Applications in Medicine (TEAM-AI). Before coming to McWilliams in 2023, Dr. Liu was the Dr. Richard F. Emslander Professor of Biomedical Informatics at Mayo Clinic and directed the Biomedical Informatics program at the Mayo Clinic Center for Clinical and Translational Science and led Cancer Data Science and Informatics of Mayo Clinic Comprehensive Cancer Center. She focuses her research on advancing translational science and bringing novel health data science, informatics, and AI solutions to empower real-world data-driven research.' 
  }, 
  { 
    id: 3, 
    name: 'Ewen M Harrison', 
    img: lu, 
    topic: 'Data Science in Surgery: Innovations and Applications',
    abstract: 'This talk will examine the intersection of data science and surgical practice, showcasing how innovative data collection and analysis methods are transforming surgical care. We will explore the use of wearable technology, automated data processing, and decision modeling in improving surgical outcomes and patient care.',
    content: 'Ewen M Harrison is a Professor of Surgery and Data Science at the University of Edinburgh and a Consultant HPB and Transplant Surgeon at the Royal Infirmary of Edinburgh. His interests include crowd-sourcing patient-level data; surgical trials, particularly in low resource settings; mobile data collection platforms and "wearables"; automated data processing and display; decision modeling; and patient-reported outcomes.' 
  },
])
</script>

<style scoped lang="less">
.speaker {
  margin-top: 110px;
  margin-bottom: 98px;
  .InvitedSpeakerList{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    .info-detail {
      margin-top: 20px;
      font-family: "TimesNewRomanPSMT", sans-serif;
      min-width: 300px;
      font-size: 20px;
      color: #2C2F31;
      line-height: 1.8;
      text-align: justifyLeft;
      font-style: normal;
      text-transform: none;
      padding: 0 16px;
      .topic {
        font-weight: bold;
        margin-bottom: 10px;
        color: #1a1a1a;
      }
      .abstract {
        margin: 15px 0;
        padding: 15px;
        background-color: #f8f9fa;
        border-left: 4px solid #2C2F31;
        .abstract-title {
          font-weight: bold;
          margin-bottom: 8px;
          color: #1a1a1a;
        }
        .abstract-content {
          font-style: italic;
          font-size: 18px;
          line-height: 1.6;
        }
      }
      .bio {
        margin-top: 15px;
        .bio-title {
          font-weight: bold;
          color: #1a1a1a;
          display: inline;
        }
        .bio-content {
          display: inline;
          line-height: 1.8;
        }
      }
    }
    & + .InvitedSpeakerList{
      padding-top: 40px;
    }
  }
}
</style>
