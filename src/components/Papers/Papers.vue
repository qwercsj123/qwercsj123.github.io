<template>
  <Page mode="dark">
    <div class="papers" id="CallForPapers">
      <div class="c-title">CALL FOR PAPERS</div>
      <div class="aim">Aims and Scope</div>
      <div class="c-paragraph ">We are inviting contributions to our workshop on "Advancing Data for Better Health:
        Reliable LLM Application in People-Centric Healthcare", focusing on four pivotal tracks.</div>
      <div class="title">Track 1: Reliability and Validation in Clinical Practice</div>
      <div class="c-paragraph">The objective of Track 1 is to ensure that LLMs provide accurate, consistent,
        and reproducible results in clinical environments, particularly for disease diagnosis and clinical decision support systems (CDSS).
        This track will discuss how theoretical frameworks of reliability can be applied in clinical practice,
        addressing the integration of real-time data streams and adaptation to rapidly changing healthcare environments.
        Additionally, methods for validating the performance of LLMs in diagnostic and decision-making applications will
        be explored to ensure their trustworthiness and mitigate risks such as misdiagnosis or treatment delays.</div>

      <div class="title">Track 2: People-Centric Interaction and Personalized Medicine</div>
      <div class="c-paragraph">Track 2 focuses on enhancing people experience, improving health literacy,
        and fostering shared decision-making through the use of LLMs in personalized healthcare.
        This track will explore how LLMs can help people understand complex medical terms, diagnostic results,
        and treatment options, as well as provide emotional support. It will also emphasize the importance of avoiding emotional manipulation
        and over-reliance on technology. Furthermore, discussions will include the design of personalized treatment plans and people education tools powered by LLMs,
        aimed at increasing people engagement and adherence to individualized healthcare interventions.</div>

      <div class="title">Track 3: Innovation and Challenges in Specific Healthcare Subfields</div>
      <div class="c-paragraph">Track 3 explores the potential applications of LLMs in specialized healthcare areas such as mental health,
        geriatric care, and drug development. This track will examine how LLMs can be used to provide emotional support in mental health care,
        manage chronic diseases in elderly patients, and accelerate drug discovery and clinical trial data analysis in pharmaceutical research.
        The session will also address challenges specific to these subfields, such as ethical concerns, data privacy issues, and technological barriers.
        Additionally, the integration of LLMs with other AI tools in healthcare will be discussed, focusing on collaborative approaches to improve outcomes.</div>

      <div class="title">Track 4: Design, Benchmarking, and Standardization</div>
      <div class="c-paragraph">Track 4 addresses the practical aspects of implementing LLMs in healthcare applications,
        focusing on user-centered design principles, performance benchmarking, and standardization.
        This track will explore how LLM-based health applications can be designed with the needs of both patients and healthcare professionals in mind,
        ensuring accessibility, usability, and effectiveness. Methods for evaluating the performance of LLMs in healthcare,
        such as establishing benchmarking practices and performance metrics, will be presented.
        Additionally, the track will highlight the importance of standardizing LLM protocols across healthcare settings to ensure consistent, high-quality results.</div>

      <div class="title">Track 5: AI and Data Applications in Healthcare</div>
      <div class="c-paragraph">Track 5 situates LLMs within the broader AI and data-driven healthcare ecosystem,
        focusing on their role in advancing personalized and intelligent healthcare solutions.
        This track will explore the integration of LLMs with AI and machine learning in healthcare informatics,
        including their contribution to data analysis, predictive modeling, and clinical decision support.
        Discussions will also cover biomedical data mining and how LLMs can assist in uncovering new insights from complex healthcare data.
        Furthermore, the track will address emerging technologies in patient care, such as remote monitoring and AI-powered health assistants,
        as well as computational methods for personalized health.</div>

      <div class="c-paragraph">Through these tracks, we aim to foster discussions and developments that will drive the integration of LLMs into people-centric healthcare.
        By addressing key areas such as ensuring the reliability of LLMs in clinical practice,
        enhancing patient interaction through personalized healthcare tools, and exploring the innovative applications of LLMs in specialized healthcare subfields,
        we will work to create a framework for the responsible and effective use of LLMs. Ultimately, the goal is to advance the use of data-driven,
        AI-powered healthcare solutions, fostering a future where LLMs play a central role in improving health outcomes and enhancing the patient experience.</div>

      <div class="aim">Paper Submission</div>

      <div class="c-paragraph">Submissions should consist of 3-8 pages for the main text, using the IEEE style file and can have unlimited space for the appendix.
        All accepted papers will be non-archival, and each submission will be rigorously assigned to at least 2-3 reviewers in a double-blind manner.
        We will use mechanisms provided by the CyberChair to handle any conflicts of interest appropriately. </div>


      <div class="c-paragraph c-break-all">
        <span class="text-bold-darkred">You can download the format instruction here: </span><span class="c-text-blue" @click="toReview('https://www.ieee.org/conferences/publishing/templates')">https://www.ieee.org/conferences/publishing/templates</span>
      </div>

      <div class="c-paragraph">
        <span class="text-bold-darkred">Attention: </span>Electronic submissions in PDF format are required.
      </div>

      <div class="c-paragraph ">
        All the papers are required to be submitted via the <span class="c-text-blue c-text-line" @click="toReview('https://wi-lab.com/cyberchair/2025/bibm25/scripts/submit.php?subarea=S36&undisplay_detail=1&wh=/cyberchair/2025/bibm25/scripts/ws_submit.php')">CyberChair</span> system.
      </div>

      <div class="c-paragraph c-break-all">
        <span class="text-bold-darkred"></span>Papers should be submitted to <span class="c-text-blue" @click="toReview('https://wi-lab.com/cyberchair/2025/bibm25/scripts/submit.php?subarea=S36&undisplay_detail=1&wh=/cyberchair/2025/bibm25/scripts/ws_submit.php')">https://wi-lab.com/cyberchair/2025/bibm25/scripts/submit.php?subarea=S36&undisplay_detail=1&wh=/cyberchair/2025/bibm25/scripts/ws_submit.php</span>
      </div>

      <div class="c-paragraph">
        The accepted papers have opportunities to be invited for submission to Health Data Science, a Science Partner Journal.
      </div>
    </div>




    <div id="KeyDates" class="key-date" style="margin-top: -40px">
      <div class="c-title">Important Dates</div>
      <div class="c-s-title notification-row">
        <span style="text-align: center"> Paper Submission Deadline: </span>
        <span class="c-inline-text">June 4, 2024</span>
<!--        <div>-->
<!--          <div class="c-inline-text" style="text-decoration: line-through;text-align: center">May 28, 2024(23:59, Anywhere on Earth)</div>-->
<!--          <div class="c-inline-text" style="padding-top: 10px;text-align: center">June 4, 2024</div>-->
<!--        </div>-->
      </div>
      <div class="c-s-title notification-row" style="margin-left: -50px">
        <span>Author Notification:</span>
        <span class="c-inline-text">June 28, 2024</span>
      </div>

      <div class="c-s-title notification-row" style="margin-left: -100px">
        <span>Camera Ready:</span>
        <span class="c-inline-text">June 28, 2024</span>
      </div>
      <div class="c-s-title notification-row" style="margin-left: -120px">
        <span>Workshop:</span>
        <span class="c-inline-text">August 26, 2024</span>
      </div>
    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
const toReview = (url)=>{
  window.open(url,"__blank")
}
</script>

<style scoped lang="less">
.key-date {
  .c-title {
    margin-bottom: 32px;
    text-align: center;
  }
  .c-s-title{
    font-size: 18px;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;

    &.notification-row {
      flex-direction: row;
      justify-content: center;
      gap: 8px;
    }
  }
  margin-bottom: 100px;
}

.c-inline-text{
  padding-left: 0;
  font-family: "HarmonyOS_Sans_SC", sans-serif;
  font-weight: normal;
  text-align: center;
}
.papers {
  margin-top: 110px;
  margin-bottom: 160px;
}
.text-bold-darkred {
  font-weight: bold; /* 设置字体加粗 */
  color: darkred;    /* 设置暗红色 */
}
.aim{
  font-size: 24px;
  color: #2c2f31;
  font-weight: bold;
  font-style: normal;
  margin-bottom: 22px;
  display: flex;
  padding: 0 16px;
}
.title {
  padding: 0 16px;
  font-family: HarmonyOS_Sans_SC_Black;
  font-size: 20px;
  color: #2c2f31;
  font-weight: bold;
  font-style: normal;
  margin-bottom: 22px;
  display: flex;
}
</style>
