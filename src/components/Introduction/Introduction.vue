<template>
  <Page>
    <div class="introduction" id="Intro">
      <div class="c-title">Introduction</div>
      <div class="c-paragraph"> Large Language Models (LLMs) present transformative potential for the healthcare sector, poised
        to revolutionize areas from medical education and clinical decision support to healthcare management.
        While these technologies can process vast medical literature, assist in diagnosis, and facilitate personalized interactions,
        their practical and widespread adoption in high-stakes healthcare environments critically hinges on their reliability.
        The promise of LLMs to elevate medical research and enhance healthcare efficiency and accuracy can only be realized if they are demonstrably safe,
        robust, and trustworthy.
      </div>
      <div class="c-paragraph">
        In parallel, People-Centered AI (PCAI) is rightly gaining prominence, emphasizing that AI systems must prioritize human needs,
        values, and capabilities. In healthcare, this means designing AI that augments clinicians, empowers patients, ensures fairness,
        mitigates bias, and involves users throughout its lifecycle.
        A people-centric approach is fundamental to building trust and ensuring that LLM applications genuinely serve patient well-being and enhance individual autonomy.
      </div>
      <div class="c-paragraph">However, the path to deploying reliable LLMs in medicine is fraught with challenges. Issues such as hallucinations,
        inherent biases, lack of transparency, irreproducibility, and data privacy concerns significantly impede their trustworthy application.
        The reliability and fairness of LLMs are intrinsically linked to the data they are trained on. Therefore,
        "Advancing Data" is central to this workshop: we will explore how optimizing data quality, ensuring data representativeness and impartiality,
        and implementing robust data governance are paramount to enhancing the applied value and, crucially, the reliability of LLMs in healthcare.
        Only through better data can we build LLMs that are not just functionally powerful but also consistently safe and universally beneficial.
      </div>
      <div class="c-paragraph">This workshop aims to bring together researchers, data scientists, clinicians, ethicists, and other stakeholders.
        We will collaboratively discuss cutting-edge research, identify critical challenges to achieving reliable LLMs, and foster interdisciplinary solutions.
        The core objective is to explore and promote innovative computational methods, rigorous data governance strategies,
        and robust evaluation frameworks specifically designed for the development and deployment of reliable, ethical,
        and effective people-centric LLM applications in healthcare, ultimately advancing data for better health outcomes.
      </div>

    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
</script>

<style scoped lang="less">
.introduction {
  padding: 38px 0 94px 0;
}
</style>
