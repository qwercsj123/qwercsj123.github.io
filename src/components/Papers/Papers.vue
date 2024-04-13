<template>
  <Page mode="dark">
    <div class="papers" id="CallForPapers">
      <div class="c-title">CALL FOR PAPERS</div>
      <div class="c-paragraph ">We are inviting contributions to our workshop on ``AI and Data Science for Healthcare: Bridging Data-centric AI and People-Centric Healthcare'', focusing on four pivotal tracks.</div>
      <div class="c-s-title">Track 1: Data-Centric AI Innovations in Healthcare</div>
      <div class="c-paragraph">This track seeks original research showcasing the use of large-scale, high-quality datasets to enhance AI model performance in healthcare settings. It focuses on bridging the gap between data volume and AI models with solutions that reflect the model's true potential, aiming to prevent overfitting and promote practical applications.</div>
      <div class="c-s-title">Track 2: People-Centric AI Technologies</div>
      <div class="c-paragraph">Submissions are invited for developing interactive, user-friendly AI technologies that boost active people participation. This track covers research on systems designed to facilitate engagement in tracking, managing, and sharing healthcare data, narrowing the gap between people's involvement and healthcare advancements.</div>
      <div class="c-s-title">Track 3: Integrated Data Systems for Personalized Medicine</div>
      <div class="c-paragraph">This track calls for papers addressing the challenge of integrating and ensuring interoperability among healthcare IT systems to bolster personalized medicine. It encourages innovative approaches to data integration, advocating for unified data standards and the utilization of diverse data types to forge comprehensive and coordinated care solutions.</div>
      <div class="c-s-title">Track 4: Explainable AI Models for Trustworthy Healthcare Decisions</div>
      <div class="c-paragraph">Contributions that focus on increasing the explainability of AI models within healthcare are welcomed in this track. It emphasizes methodologies and technologies that enhance model transparency, aiming to build trust among people and healthcare providers in AI-driven decisions.</div>
      <div class="c-paragraph">Through these tracks, we aim to foster discussions and developments that push the boundaries of AI and Data Science in healthcare, enhancing both diagnostic accuracies and fostering a people-centric approach to healthcare innovation.</div>
      <div class="c-paragraph">Submissions to this KDD conference should consist of a main text of up to 5 pages using the ACM style file, with unlimited space allowed for the appendix. All papers must be non-archival, and submissions will undergo a rigorous double-blind review process by at least 2-3 assigned reviewers using OpenReview to manage any conflicts of interest effectively. Author names and affiliations should not be listed to adhere to the double-blind policy.</div>
      <div class="c-paragraph">Papers will be evaluated based on novelty, technical quality, potential impact, and clarity of writing. Substantial emphasis is placed on empirical evaluations; therefore, experimental methods and results must be clear, well-executed, and repeatable. Authors are strongly encouraged to make their data and code publicly available. Accepted papers will be posted on the workshop website but will not be included in the KDD proceedings.</div>
      <div class="c-paragraph">One recommended setting for Latex file of anonymous manuscript is: \documentclass[sigconf, anonymous, review]{acmart}. Template guidelines are here: <span class="c-text-blue" @click="toReview('https://www.acm.org/publications/proceedings-template')">https://www.acm.org/publications/proceedings-template</span></div>
      <div class="c-paragraph"> All the papers are required to be submitted via the <span
          class="c-text-blue c-text-line" @click="toReview('https://openreview.net/group?id=KDD.org/2024/Workshop/AIDSH&referrer=%5BHomepage%5D(%2F)#tab-your-consoles')">OpenReview</span> system.
      </div>

      <div class="c-paragraph c-break-all">
        <span class="c-text-blue" @click="toReview('https://openreview.net/group?id=KDD.org/2024/Workshop/AIDSH&referrer=%5BHomepage%5D(%2F)#tab-your-consoles')">https://openreview.net/group?id=KDD.org/2024/Workshop/AIDSH&referrer=%5BHomepage%5D(%2F)#tab-your-consoles</span>
      </div>
      <div class="c-paragraph">
        The accepted papers have opportunities to be invited for submission to <span style="font-style: italic; font-weight: 600;">Health Data Science</span>, a Science Partner Journal.
      </div>
      <div class="c-paragraph">
        Any questions may be directed to the email address: hongshenda@pku.edu.cn
      </div>
    </div>
    <div id="KeyDates" class="key-date">
      <div class="c-title">Key Dates</div>
      <div class="c-s-title">
        <span > Paper Submission Deadline: </span><span class="c-inline-text">May 28, 2024(23:59, Anywhere on Earth)</span></div>
      <div class="c-s-title">Author Notification:<span class="c-inline-text">June 28, 2024</span></div>
      <div class="c-s-title">Workshop:<span class="c-inline-text">August 26, 2024</span></div>
    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
const toReview = (url)=>{
  window.open("https://openreview.net/group?id=KDD.org/2024/Workshop/AIDSH&referrer=%5BHomepage%5D(%2F)#tab-your-consoles","__blank")
}
</script>

<style scoped lang="less">
.key-date {
  .c-title {
    margin-bottom: 16px;
  }
  .c-s-title{
    font-size: 18px;
  }
  margin-bottom: 100px;
}

.c-inline-text{
  padding-left: 6px;
  font-family: "HarmonyOS_Sans_SC", sans-serif;
  font-weight: normal;
}
.papers {
  margin-top: 110px;
  margin-bottom: 160px;
}
</style>
