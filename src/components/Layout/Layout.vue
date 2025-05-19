<template>
  <div class="layout">
    <Anchor></Anchor>
    <Banner></Banner>
    <Introduction></Introduction>
    <Schedule></Schedule>
    <Speaker></Speaker>
    <AcceptedPapers></AcceptedPapers>
    <Papers></Papers>
<!--    <Steering></Steering>-->
    <ProgramCom></ProgramCom>
    <Operational></Operational>
    <Sponsors></Sponsors>
  </div>
</template>

<script setup>
import Banner from "../Banner/Banner.vue"
import Introduction from "../Introduction/Introduction.vue";
import Speaker from "../Speaker/Speaker.vue";
import AcceptedPapers from "../AcceptedPapers/AcceptedPapers.vue";
import Papers from "../Papers/Papers.vue";
import Steering from "../Steering/Steering.vue";
import ProgramCom from "../Program/ProgramCom.vue";
import Operational from "../Operational/Operational.vue";
import Sponsors from "../Sponsors/Sponsors.vue";
import Anchor from "@/components/Anchor/Anchor.vue";
import Schedule from "@/components/Schedule/Schedule.vue";
</script>

<style scoped lang="less">
.layout {
  overflow-x: hidden;
}
</style>