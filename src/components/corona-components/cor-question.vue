<script>
import DiseaseQu from './Question-component/disease.vue'
import BustersQu from './Question-component/busters-qu.vue'
import CommunityQu from './Question-component/community-qu.vue'
import ProtactQu from './Question-component/protact-qu.vue'
import SpreadQu from './Question-component/spreads-qu.vue'
import TestingQu from './Question-component/testing-qu.vue'
export default {
    components: {
        DiseaseQu,
        BustersQu,
        CommunityQu,
        ProtactQu,
        SpreadQu,
        TestingQu,
    },
    data(){
        return{
            awesome:1,
        }
    },
    methods:{

    },
};
</script>

<template>
    <section class="question py-5 mt-5" id="question">
        <div class="container">
            <div class="main-title">
                <h2 class="mb-3">common question & answer</h2>
            </div>
            <div class="row">
                <div class="col-md-3">
                    <div class="buttons">
                        <button @click="awesome=1" id="btn1" :class="['btn', 'btn-outline-light', 'shadow', 'text-dark', 'mb-3', 'P-2',awesome== 1?'active':'']">CoraneVirus Disease 2019 Basics <i class="bi bi-caret-right-fill"></i></button>

                        <button @click="awesome=2" id="btn2" :class="['btn', 'btn-outline-light', 'shadow', 'text-dark', 'mb-3', 'P-2',awesome== 2?'active':'']">How It Spreads <i class="bi bi-caret-right-fill"></i></button>

                        <button @click="awesome=3" id="btn3" :class="['btn', 'btn-outline-light', 'shadow', 'text-dark', 'mb-3', 'P-2',awesome==3 ?'active':'']">How To Protact YourSelf <i class="bi bi-caret-right-fill"></i></button>

                        <button @click="awesome=4" id="btn4" :class="['btn', 'btn-outline-light', 'shadow', 'text-dark', 'mb-3', 'P-2',awesome==4 ?'active':'']">Symptoms & Testing <i class="bi bi-caret-right-fill"></i></button>

                        <button @click="awesome=5" id="btn5" :class="['btn', 'btn-outline-light', 'shadow', 'text-dark', 'mb-3', 'P-2',awesome== 5?'active':'']">Outbreak in Your Community <i class="bi bi-caret-right-fill"></i></button>

                        <button @click="awesome=6" id="btn6" :class="['btn', 'btn-outline-light', 'shadow', 'text-dark', 'mb-3', 'P-2',awesome== 6 ?'active':'']">Myth-Busters of CoronaVirus <i class="bi bi-caret-right-fill"></i></button>
                    </div>
                </div>
                <div class="col-md-8">
                    <div class="answers text-dark" id="answers">
                        <DiseaseQu v-if="awesome==1" id="ans1"></DiseaseQu>
                        <BustersQu v-if="awesome==2" id="ans2"></BustersQu>
                        <CommunityQu v-if="awesome==3" id="ans3"></CommunityQu>
                        <ProtactQu v-if="awesome==4" id="ans4"></ProtactQu>
                        <SpreadQu v-if="awesome==5" id="ans5"></SpreadQu>
                        <TestingQu v-if="awesome==6" id="ans6"></TestingQu>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<style scoped>
.main-title h2::before{
    content: "frequently asked question";
}
.active{
    color: var(--main-color) !important;
    border-color: var(--main-color) !important;
}
.question .buttons{
    display: flex;
    flex-direction: column;
    
}
.question .buttons button{
    text-align: left;
    display: flex;
    justify-content: space-between;
}
.question .buttons button:focus{
    border-color: var(--main-color);
    color: var(--main-color) !important;
}
.question .answers{
    border: 1px solid #00000048;
}
@media (max-width: 767px) {
    *{
        padding: 0%;
        margin: 0%;
    }
}
</style>