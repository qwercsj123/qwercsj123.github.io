<template>
    <Page>
        <div class="acceptedPapers" id="AcceptedPapers">
            <div class="c-title">Accepted Papers</div>
            <div class="c-paragraph" style="text-align: center; font-weight: bold; font-size: 25px;">Oral</div>
            <table>
                <tr>
                <td class="flex-center font-weight">Title</td>
                <td class="flex-center font-weight">Author</td>
                <td class="flex-center font-weight">Link</td>
                </tr>
                <tr v-for="(item, index) in listData" :key="index">
                    <td>{{ item.title }}</td>
                    <td>{{ item.author }}</td>
                    <td>{{ item.link }}</td>
                </tr>
            </table>

            <div class="c-paragraph" style="text-align: center; font-weight: bold; font-size: 25px;">Poster</div>
            <table>
                <tr>
                <td class="flex-center font-weight">Title</td>
                <td class="flex-center font-weight">Author</td>
                <td class="flex-center font-weight">Link</td>
                </tr>
                <tr v-for="(item, index) in listData" :key="index">
                    <td>{{ item.title }}</td>
                    <td>{{ item.author }}</td>
                    <td>{{ item.link }}</td>
                </tr>
            </table>
        </div>
    </Page>
</template>

<script setup>
import { ref } from "vue";

const listData = ref([
    { title: "R&B -  Rhythm and Brain: Cross-subject decoding of musical tracks from human brain activity", author: "Matteo Ferrante, Matteo Ciferri, Nicola Toschi", link: "" },
    { title: "EHRFlow: A Large Language Model-Driven Iterative Multi-Agent Electronic Health Record Data Analysis Workflow", author: "Hao Wu, Yinghao Zhu, Junyi Gao, Zixiang Wang, Xiaochen Zheng, Yasha Wang, Ewen M Harrison, Chengwei Pan, Liantao Ma", link: "" },
    { title: "Faithfulness Hallucination Detection in Healthcare AI", author: "Prathiksha Rumale Vishwanath, Simran Tiwari, Tejas Ganesh Naik, Sahil Gupta, Dung Ngoc Thai, Wenlong Zhao, SUNJAE KWON, Victor Ardulov, Karim Tarabishy, Andrew McCallum, Wael Salloum", link: "" },
    { title: "REINVENT-Transformer: Molecular De Novo Design through Transformer-based Reinforcement Learning", author: "Pengcheng Xu, Tianfan Fu, Wenhao Gao, Jimeng Sun", link: "" },
    { title: "Reading Your Heart: Learning ECG Words and Sentences via Pre-training ECG Language Model", author: "Jiarui Jin, Haoyu Wang, Jun Li, Sichao Huang, Jiahui Pan, Shenda Hong", link: "" },
    { title: "Hybrid AI Approach for Counterfactual Prediction over Knowledge Graphs for Personal Healthcare", author: "Hao Huang, Emetis Niazmand, Maria-Esther Vidal", link: "" },
    { title: "Effectiveness of a digital quantitative assessment of protein-to-creatinine ratio using computer-vision technologies in proteinuria screening", author: "Jingyi Wu, Yuewen Zheng, Chunmiao Zhou, Fei Wang, Qing Li, Pengfei Li, Luxia Zhang", link: "" },
    { title: "State Space Model-based Classification of Major Depressive Disorder Across Multiple Imaging Sites", author: "Shusheng Li, Bo Yang, Ting Ma, Chenfei Ye", link: "" },
    { title: "In Medical Claims Data, Enhancing Predictive Performance for Major Adverse Cardiovascular Events Using Cross Attention", author: "Yuhei Fujioka, Daitaro Misawa, Tatsuyoshi Ikenoue, Shingo Fukuma ", link: "" },
    { title: "How well do simulated populations with GPT-4 align with real ones in clinical trials? The case of the EPQR-A personality test", author: "Jose Gregorio Ferreira De Sá, Andreas Kaltenbrunner, Jacopo Amidei, Rubén Nieto", link: "" },
    { title: "Bayesian Disease Progression Modeling That Accounts for Health Disparities", author: "Erica Chiang, Ashley N. Beecy, Gabriel Sayer, Nir Uriel, Deborah Estrin, Nikhil Garg, Emma Pierson", link: "" },
])
const posterListData = ref([
    {title: "Dynamic Graph and Multi-view Medication Information for Recommending Medication Combination", author: "Guanlin Liu", link: ""},
    {title: "RetCare: Towards Interpretable Clinical Decision Making through LLM-Driven Medical Knowledge Retrieving", author: "Zixiang Wang, Yinghao Zhu, Junyi Gao, Xiaochen Zheng, Yuhui Zeng, Yasha Wang, Ewen M Harrison, Chengwei Pan, Liantao Ma", link: ""},
    {title: "Reinforcement Learning-based Decision-making for Renal Replacement Therapy in ICU-acquired AKI Patients", author: "Haoyuan Zhang, Minqi Xiong, Tongyue Shi, Wentie Liu, Haowei Xu, Huiying Zhao, Guilan Kong", link: ""},
    {title: "Constructing a knowledge-driven and data-driven hybrid decision model for etiological diagnosis of Ventricular Tachycardia", author: "Min Wang, Zhao Hu, Xiaowei Xu, Si Zheng, Jiao Li, Yan Yao ", link: ""},
    {title: "DiffuSETS: 12-lead ECG Generation Conditioned on Clinical Text Reports and Patient-Specific Information", author: "Jiabo Chen, Yongfan Lai, Deyun Zhang, yuewang, Shijia Geng, Hongyan Li, Shenda Hong ", link: ""},
    {title: "A Predictive Model for Real-time Prediction of Intradialytic Hypotension Based on Machine Learning Algorithms", author: "Jiang Yuping, Bian Xueqin, Hong Xueming, Si Haiyan, Liu Di, Chen Hao", link: ""},
    {title: "Take Your Steps: Hierarchically Efficient Pulmonary Disease Screening via CT Compression", author: "Qian Shao, Kai Zhang, Bang Du, Zepeng Li, Yixuan Wu, Qiyuan Chen, Jian Wu, Jintai Chen ", link: ""},
    {title: "DeepEST: A Python Libary for Spatio-Temporal Epidemiology Prediction", author: "Yuhang Wang, Junyi Gao, Yinghao Zhu, Lifang Liang, Yasha Wang, Ewen M Harrison, Liantao Ma", link: ""},
    {title: "Language Interaction Network for Clinical Trial Outcome Prediction", author: "Chufan Gao, Tianfan Fu, Jimeng Sun", link: ""},
    {title: "Human-guided Rule Learning for ICU Readmission Risk Analysis", author: "Lincen Yang, Matthijs van Leeuwen", link: ""},
    {title: "JSCDS: A Core Data Selection Method with Jason-Shannon Divergence for Caries RGB Images-Efficient Learning", author: "Peiliang Zhang, Yujia Tong, Chenghu Du, Chao Che, Yongjun Zhu", link: ""},
    {title: "Identifying Subphenotypes for Sepsis with Acute Kidney Injury via Multimodal Graph State Space Models", author: "Haowei Xu, Guilan Kong, Tongyue Shi, Wentie Liu, Huiying Zhao", link: ""},
    {title: "Multi-Channel Masked Autoencoder and Comprehensive Evaluations for Reconstructing 12-Lead ECG from Arbitrary Single-Lead ECG", author: "Jiarong chen, Wanqing Wu, Shenda Hong", link: ""},
    {title: "Large Window-based Mamba UNet for Medical Image Segmentation: Beyond Convolution and Self-attention", author: "Jinhong Wang, Jintai Chen, Danny Chen, Jian Wu ", link: ""},
    {title: "PGCN-DDI: Drug-Drug Interaction Prediction Based on Multidimensional Drug Features and Neighborhood Overlap Similarity", author: "Wangli", link: ""},
    {title: "$$Predict the Risk of Dyslipidemia via Deep Neural Networks for Survival Data$$", author: "Jiahui Xiao", link: ""},
    {title: "Tandem: a Confidence-based Approach for Precise Medical Image Segmentation", author: "Simone Monaco, Lorenzo Petrosino, Christodoulos Xinaris, Daniele Apiletti ", link: ""},
    {title: "Decentralized Diagnosis: Privacy-Preserving Brain Tumor Classification with Federated Learning", author: "Chaima Lhasnaoui, Addi Ait-Mlouk, Tarik Agouti, Mohammed Sadgal ", link: ""},
    {title: "TeleOR: Real-time Full-Scene Operating Room Telemedicine System", author: "Yixuan Wu, Kaiyuan Hu, Qian Shao, Danny Chen, Jian Wu, Jintai Chen", link: ""},
    {title: "Using Large Language Models to Detect Outcomes in Qualitative Studies on Adolescent Depression", author: "Alison W. Xin, Dylan Nielson, Karolin Krause, Guilherme Fiorini, Nick Midgley, Francisco Pereira, Juan Antonio Lossio-Ventura", link: ""},
    {title: "Artificial Intelligence in Traditional Chinese Medicine: P+C36ast, Present and Future", author: "Tian Xu, Liqiang Ni ", link: ""},
    {title: "Hybrid Deep Learning Framework for Enhanced Melanoma Detection", author: "Peng Zhang, Divya Chaudhary ", link: ""},
    {title: "Velocity-based training assessment: Effect of Extended-Relative-Phase-based extracted features on classification", author: "Yeong Ju Woo, Hang Thi Phuong Nguyen, Hieyong Jeong ", link: ""},
    {title: "HPExplainPro: A Framework for Pan-cancer Prognosis Prediction Based on Deep Interpretable Learning", author: "Houwu GONG, Zhijian Huang, Min Jin", link: ""},
    {title: "Development and Validation of an Explainable Machine Learning-Based Model for Predicting the Interval Growth of Pulmonary Subsolid Nodules: A Prospective Multicenter Cohort Study", author: "Zhedong Zhang", link: ""},
    {title: "Cluster analysis of multimorbidity and healthcare burden based on machine learning: results from CHARLS", author: "Huizhao ", link: ""},
    {title: "Selecting an Effective Sequential Transfer Path for Medical Image Segmentation", author: "Yang Jingyun", link: ""},
])
</script>

<style scoped lang="less">
.acceptedPapers {
    margin-bottom: 100px;
    table {
        border-collapse: collapse;
        max-width: 1000px;
        border-left: 1px solid #4d4d4d;
        border-top: 1px solid #4d4d4d;
        margin: 0 auto;
        font-family: "TimesNewRomanPSMT", sans-serif;
        font-size: 22px;
        color: #2C2F31;
        tr{
            display: flex;
            td{
                flex: 1;
                border-right: 1px solid #4d4d4d;
                border-bottom: 1px solid #4d4d4d;
                min-height: 30px;
                padding: 8px;
                overflow: hidden;
            }
        }
        .flex-center{
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .font-weight{
            font-weight: bold;
        }
    }
}
</style>