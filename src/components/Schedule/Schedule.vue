<template>

    <div class="schedule" id="Schedule">
      <div style=" background-color: #EEE;height: 80px"></div>
      <div class="c-title">SCHEDULE</div>
      <div class="dataAndLocation" >
        <h3 >1:00 PM - 5:00 PM (PT)</h3>
        <h3>Venue: 201A </h3>
      </div>
      <div class="container">

        <div class="row">
          <div class="col-lg-1 text-left" >
            &nbsp;
          </div>

          <div class="content">

            <p >01:00-01:15 Opening remarks</p>
            <p>01:15-2:00 Keynote Talk </p>
            <ul>
              <li><strong> Robust and Intelligent Time Series Analysis and Applications </strong>, <em>Prof. Wotao Yin</em></li>
            </ul>

            <p>2:50-2:45 Keynote Talk </p>
            <ul>
              <li><strong> Modeling Temporal Data via Knowledge-Guided Machine Learning: A New Framework for Accelerating Scientific Discovery and Addressing Global Environmental Challenges
              </strong>, <em>Prof. Vipin Kumar</em></li>
            </ul>

            <p>2:45-3:30 Poster Session + Coffee Break</p>
            <p>3:30-4:10 Contributed Talks </p>
            <ul>
              <li>
                <strong>Deep Sequence Modeling for Event Log-based Predictive Maintenance</strong>.<em>Yun Zhou, Yawei Wang, Huan Song, Tesfagabir Meharizghi, Mohamad Al Jazaery, Denisse Colin-Magana, Aruna Abeyakoon and Panpan Xu.</em> </li>
              <li>
                <strong>Dynamic Ensemble for Probabilistic Time-series forecasting via Deep Reinforcement Learning</strong>. <em>Ding, Youngsuk Park, Karthick Gopalswamy, Hilaf Hasson, Yuyang Wang and Jun Huan.</em> </li>
              <li>
                <strong>VQ-TR: Vector Quantized Attention for Time Series Forecasting</strong>.<em>Kashif Rasul, Umang Gupta, Hena Ghonia, Anderson Schneider and Yuriy Nevmyvaka.</em> </li>
              <li>
                <strong>Long-Range Transformers for Dynamic Spatiotemporal Forecasting</strong>. <em>Grigsby, Zhe Wang, Nam H Nguyen and Yanjun Qi.</em>
              </li>

              <li>
                <strong> STNN-SDE: Continuous Stochastic Spatial-Temporal Representation Learning via Latent Stochastic Differential Equations</strong>.<em>Yanbo Xu, Piyush Patil, Lingkai Kong and Chao Zhang.</em> </li>
            </ul>



            <p>4:10-4:55 pm Keynote Talk </p>
            <ul>
              <li><strong>Convolutional kernels for effective and scalable time series analytics</strong>, <em>Prof. Geoff Webb</em></li>
            </ul>

            <p>4:55-5:00 pm Concluding Remarks</p>

          </div>

        </div>

        <div style=" background-color: #EEE;height: 80px"></div>
      </div>

    </div>

</template>

<script setup>
import Page from "../Page/Page.vue"
</script>

<style scoped lang="less">
.schedule {
  margin-top: 110px;
  margin-bottom: 80px;
  background-color: #EEE
}


.row{
  margin-right:-15px;
  margin-left:-15px
}
.content p{
  font-size: 14px;
  line-height: 1.75;
  color: #333;
  margin: 0 0 10px;
}

.content ul li strong{
  font-weight: 700;
  font-size: 14px;
  line-height: 1.42857143;
  color: #333;
}

.content ul li em{
  font-style: italic;
  font-size: 14px;
  line-height: 1.42857143;
  color: #333;
}

.container{
  padding-right:15px;
  padding-left:15px;
  margin-right:auto;
  margin-left:auto;
}


@media only screen and (min-width: 400px) and (max-width: 960px) {
  .content p {
    font-size: 14px;
    line-height: 1.75;
    color: #333;
    padding-left: 15px;
  }
}

@media (min-width:992px) {
  .container{
    width:970px
  }
}

@media (min-width:1200px){
  .container {
    width:1170px
  }
}
.dataAndLocation{
  text-align: center;
}
.dataAndLocation h3{
  font-family: Montserrat, "Helvetica Neue", Helvetica, Arial, sans-serif;
  text-transform: uppercase;
  font-weight: 700;
  margin-top: 20px;
  margin-bottom: 10px;
  line-height: 1.1;
  color: #333;
}

.dataAndLocation h4{
  font-family: Montserrat, "Helvetica Neue", Helvetica, Arial, sans-serif;
  text-transform: uppercase;
  font-weight: 700;
  margin-top: 20px;
  margin-bottom: 10px;
  line-height: 1.1;
  color: #333;
}


</style>
