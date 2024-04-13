<template>
  <Page mode="dark">
    <div class="papers" id="CallForPapers">
      <div class="c-title">CALL FOR PAPERS</div>
      <div class="c-paragraph ">We are inviting contributions to our workshop on "AI and Data Science for Healthcare:
        Bridging Data-centric
        AI and People-Centric Healthcare", focusing on four pivotal tracks.</div>
      <div class="c-paragraph">Firstly, we're looking for original research in "Data-Centric AI Innovations in
        Healthcare," which showcases
        leveraging large-scale, high-quality datasets to enhance AI model performance in healthcare settings, aiming to
        bridge the gap between data volume and AI models with solutions that reflect the model's true potential beyond
        mere overfitting.</div>
      <div class="c-paragraph">Secondly, the "People-Centric AI Technologies" track seeks submissions on developing
        interactive, user-friendly
        AI technologies designed to boost active people participation. This includes research on systems that facilitate
        people's engagement in tracking, managing, and sharing their healthcare data, thereby narrowing the gap between
        people's involvement and healthcare.</div>
      <div class="c-paragraph">Thirdly, "Integrated Data Systems for Personalized Medicine" calls for papers addressing
        the challenge of
        integrating and ensuring interoperability among healthcare IT systems to bolster personalized medicine. We
        encourage innovative approaches to data integration, advocating for unified data standards and the utilization
        of diverse data types to forge comprehensive and coordinated care solutions.</div>
      <div class="c-paragraph">Lastly, the "Explainable AI Models for Trustworthy Healthcare Decisions" track welcomes
        contributions that focus
        on increasing the explainability of AI models within healthcare. This track emphasizes methodologies and
        technologies that enhance model transparency, aiming to build trust among people and healthcare providers in
        AI-driven decisions.</div>
      <div class="c-paragraph">Through these tracks, we aim to foster discussions and developments that push the
        boundaries of AI and Data
        Science in healthcare, enhancing both diagnostic accuracies and fostering a people-centric approach to
        healthcare innovation.</div>
      <div class="c-paragraph">Submissions should consist of 3-8 pages for the main text, using the ACM style file and
        can have unlimited space
        for the appendix. All accepted papers will be non-archival, and each submission will be rigorously assigned to
        at least 2-3 reviewers in a double-blind manner. We will use mechanisms provided by the OpenReview to handle any
        conflicts of interest appropriately.</div>
      <div class="c-paragraph">One recommended setting for Latex file of anonymous manuscript is:
        \documentclass[sigconf,
        anonymous,
        review]{acmart}. Template guidelines are here: https://www.acm.org/publications/proceedings-template.</div>
      <div class="c-paragraph">Following this KDD conference submission policy, reviews are double-blind, and author
        names and affiliations
        should NOT be listed. Submitted papers will be assessed based on their novelty, technical quality, potential
        impact, and clarity of writing. For papers that rely heavily on empirical evaluations, the experimental methods
        and results should be clear, well-executed, and repeatable. Authors are strongly encouraged to make data and
        code publicly available whenever possible. The accepted papers will be posted on the workshop website but will
        not be included in the KDD proceedings.</div>
      <div class="c-paragraph">Please note that at least one of the authors of each accepted paper must register for the
        workshop and attend in
        person to present the paper during the workshop.</div>
      <div class="c-paragraph"> All the papers are required to be submitted via the <span
          class="c-text-blue" @click="toReview">OpenReview</span> system.
      </div>
      <div class="c-paragraph c-break-all">
        https://openreview.net/group?id=KDD.org/2024/Workshop/AIDSH&referrer=%5BHomepage%5D(%2F)#tab-your-consoles
      </div>
      <div class="c-paragraph">
        The accepted papers have opportunities to be invited for submission to Health Data Science, a Science Partner
        Journal.
      </div>
    </div>
    <div id="KeyDates" class="key-date">
      <div class="c-title">Key Dates</div>
      <div class="c-s-title">
        <span > Paper Submission Deadline: </span><span class="c-inline-text">May 28, 2024: Workshop paper submission due (23:59, Anywhere on Earth)</span></div>
      <div class="c-s-title">Author Notification:<span class="c-inline-text">June 28, 2024: Workshop paper notifications</span></div>
      <!-- <div class="c-s-title">Camera Ready Version:<span class="c-inline-text">August 26, 2024: Workshop date</span></div> -->
      <div class="c-s-title">Workshop:<span class="c-inline-text">August 26, 2024: Workshop date</span></div>
    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
const toReview = ()=>{
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
