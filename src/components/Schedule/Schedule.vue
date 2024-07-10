<template>
  <Page mode="">
    <div class="schedule" id="Schedule">
      <div class="c-title">SCHEDULE</div>
      <div class="c-paragraph" style="text-align: center;font-weight: bold;font-size: 25px">August 26, 2024 </div>
      <div class="c-paragraph"style="text-align: center;font-weight: bold;font-size: 25px" > Location: TBD </div>
      <div class="c-paragraph" style="text-align: center;font-weight: bold;font-size: 25px"> Zoom Link: TBD </div>
        
     
  <table>
    <tr>
      <td>Time(GMT+8)</td>
      <td>Title</td>
    </tr>
    <tr>
        <td>2:00 pm - 2:10 pm</td>
        <td>Introduction and welcome</td>
    </tr>
    <tr>
        <td>2:10 pm - 3:40 pm</td>
        <td>Invited Talks</td>
    </tr>
    <tr>
        <td>3:40 pm - 4:10 pm</td>
        <td>Break</td>
    </tr>
    <tr>
        <td>4:10 pm - 5:10 pm</td>
        <td>Contributed talks</td>
    </tr>
    <tr>
        <td>5:10 pm - 6:10 pm</td>
        <td>Break and Poster Session</td>
    </tr>
    <tr>
        <td>6:10 pm - 6:20 pm</td>
        <td>Closing Ceremony</td>
    </tr>
</table>

    </div>
  </Page>
</template>

<script  setup>
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
      border-collapse: collapse;
      width: 700px;
      height: 400px;
      border: 1px solid black;
      margin-left: 300px;
      }

      th, td {
        text-align: center;
        padding: 8px;
        border-bottom: 1px solid #ddd;
        border: 1px solid black;
        width: 25%;
        font-size: 23px
        }
        th {
            background-color: #f2f2f2;
            border: 1px solid black;
            font-size: 23px
        }


</style>
