<template>
  <Page mode="">
    <div class="schedule" id="Schedule">
      <div class="c-title">SCHEDULE</div>
      <div class="c-paragraph" style="text-align: center;font-weight: bold;font-size: 25px">August 26, 2024 </div>
      <div class="c-paragraph" style="text-align: center;font-weight: bold;font-size: 25px"> Location: TBD </div>
      <div class="c-paragraph" style="text-align: center;font-weight: bold;font-size: 25px"> Zoom Link: TBD </div>


      <table>
        <tr>
          <td class="flex-center">Time(GMT+8)</td>
          <td class="flex-center">Title</td>
        </tr>
        <tr>
          <td class="flex-center">2:00 pm - 2:10 pm</td>
          <td class="flex-center">Introduction and welcome</td>
        </tr>
        <tr>
          <td class="flex-center">2:10 pm - 3:40 pm</td>
          <td class="flex-center">Invited Talks</td>
        </tr>
        <tr>
          <td class="flex-center">3:40 pm - 4:10 pm</td>
          <td class="flex-center">Break</td>
        </tr>
        <tr>
          <td class="flex-center">4:10 pm - 5:10 pm</td>
          <td class="flex-center">Contributed talks</td>
        </tr>
        <tr>
          <td class="flex-center">5:10 pm - 6:10 pm</td>
          <td class="flex-center">Break and Poster Session</td>
        </tr>
        <tr>
          <td class="flex-center">6:10 pm - 6:20 pm</td>
          <td class="flex-center">Closing Ceremony</td>
        </tr>
      </table>

    </div>
  </Page>
</template>

<script setup>
import Page from "../Page/Page.vue"
</script>

<style scoped lang="less">
.schedule {
  margin-top: 110px;
  margin-bottom: 80px;
}

// table, th, td {
//   border: 1px solid black;
//   border-collapse: collapse; /* 移除单元格间的间隔 */
// }

table {
  max-width: 700px;
  border-left: 1px solid #4d4d4d;
  border-top: 1px solid #4d4d4d;
  margin: 0 auto;
}

tr {
  display: flex;

  td {
    font-size: 23px;
    flex: 1;
    border-right: 1px solid #4d4d4d;
    border-bottom: 1px solid #4d4d4d;
    min-height: 30px;
    padding: 8px;
    overflow: hidden;
  }
}

.flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.font-weight {
  font-weight: bold;
}
</style>
