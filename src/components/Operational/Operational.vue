<template>
  <Page>
    <div class="operational">
      <div class="c-title">Operational Committee</div>
      <div class="small row-two-columns" style="display: flex;margin-top: 80px">
        <div class="column-half">
          <ul>

            <li><strong>Ayan Chatterjee</strong> (Northeastern University) </li>

            <li><strong>Baixiang Huang</strong> (National University of Singapore) </li>

            <li><strong>Brandon A Mayer</strong> (Google) </li>

            <li><strong>Chen Shao</strong> (Karlsruhe Institute of Technology) </li>

            <li><strong>Chenhui Deng</strong> (Cornell University) </li>

            <li><strong>Delvin Ce Zhang</strong> (Singapore Management University) </li>

            <li><strong>Dingsu Wang</strong> (University of Illinois at Urbana-Champaign) </li>

            <li><strong>Dongjin Song</strong> (University of Connecticut) </li>

            <li><strong>Dongkwan Kim</strong> (KAIST) </li>

            <li><strong>Jian Kang</strong> (University of Rochester) </li>

            <li><strong>Jiarui Lu</strong> (Mila) </li>

          </ul>
        </div>
        <div class="column-half">
          <ul>

            <li><strong>Johannes Gasteiger</strong> (Technical University of Munich) </li>

            <li><strong>Leonardo F. R. Ribeiro</strong> (TU Darmstadt) </li>

            <li><strong>Mehdi Azabou</strong> (Georgia Institute of Technology) </li>

            <li><strong>Neil Shah</strong> (Snap Inc.) </li>

            <li><strong>Oliver Kiss</strong> (Central European University) </li>

            <li><strong>Rik Sarkar</strong> (The University of Edinburgh) </li>

            <li><strong>Shuangjia Zheng</strong> (Sun Yat-sen University) </li>

            <li><strong>Sungsoo   Ahn</strong> (POSTECH) </li>

            <li><strong>Wenqing Zheng</strong> (University of Texas at Austin) </li>

            <li><strong>Xingjian Zhang</strong> (University of Michigan) </li>

          </ul>
        </div>
      </div>
    </div>
  </Page>
</template>

<script setup>
import { ref } from 'vue'
import Info from "@/common/components/Info/Info.vue"
import Page from "../Page/Page.vue"
import yin from "@/assets/30.jpg"
import wang from "@/assets/31.jpg"
import yang from "@/assets/32.jpg"
import tang from "@/assets/36.jpg"
import gao from "@/assets/37.jpg"
import sun from "@/assets/38.jpg"
const listData = ref([
  { id: 1, name: 'Daoxin Yin', img: yin, content: 'Daoxin Yin, the Executive Editor for Health Data Science (HDS) and previously served as the China Editor for BMJ.' },
  { id: 2, name: 'Mai Wang', img: wang, content: 'Mai Wang, the Director of the Health Data Science (HDS) Editorial Office and the Head of the Comprehensive Department at National Institute of Health Data Science at Peking University.' },
  { id: 3, name: 'Yu Yang', img: yang, content: 'Yu Yang, Assistant Research Professor at National Institute of Health Data Science at Peking University.' },
  { id: 4, name: 'Gongzheng Tang', img: tang, content: 'Gongzheng Tang, PhD student in health data science at Peking University.' },
  { id: 5, name: 'Junyi Gao', img: gao, content: 'Junyi Gao, Ph.D. student in the Health Data Research UK (HDRUK) program at the University of Edinburgh.' },
  { id: 6, name: 'Chenxi Sun', img: sun, content: 'Chenxi Sun, PhD student in intelligence science and technology at Peking University.' },

])
</script>

<style scoped lang="less">
.operational {
  margin-top: 110px;
  margin-bottom: 150px;
  display: flex;
  flex-direction: column;
  align-items: center;

  .row-two-columns {
    max-width: 1000px;
    width: 100%;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;  // 允许在需要时换行
  }
}

.column-half{
  flex: 0 0 50%;  // 修改flex属性，防止挤压
  color: #3d4144;
  font-family: -apple-system, BlinkMacSystemFont, "Roboto", "Segoe UI", "Helvetica Neue", "Lucida Grande", Arial, sans-serif;
  line-height: 1.5;

  ul {
    padding: 0;
    margin: 0;
  }

  li {
    margin-bottom: 12px;
    &:last-child {
      margin-bottom: 0;
    }
  }
}

// 添加媒体查询，处理手机端显示
@media screen and (max-width: 768px) {
  .operational {
    .row-two-columns {
      flex-direction: column;
      padding-left: 40px;  // 增加左内边距到40px
    }
    
    .column-half {
      flex: 0 0 100%;
      margin-bottom: 20px;
      
      &:last-child {
        margin-bottom: 0;
      }
    }
  }
}
</style>
