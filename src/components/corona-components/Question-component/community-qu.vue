<template>
    <div class="container"><div class="contain">
        <div :class="['community' ,open[0]?'active':'']">
            <h6>who Lorem ipsum dolor sit amet consectetur?</h6>
            <div class="button" @click="change">
                <h3 data-num="0">{{open[0]? '-': '+'}}</h3>
            </div>
        </div>
        <div class="answer" v-if="open[0]">
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odio ea ipsa molestias illum dolor laboriosam dolorum obcaecati magnam minus nisi. Atque porro veritatis neque magni in autem amet a, vitae aliquid doloremque deleniti cumque, perspiciatis consectetur mollitia deserunt facilis, sequi hic nobis voluptatem nemo labore quam? Amet veniam repellendus aliquid.</p>
        </div>
    </div>
    <div class="contain">
        <div :class="['community' ,open[1]?'active':'']">
            <h6>who Lorem ipsum dolor sit amet consectetur?</h6>
            <div class="button" @click="change">
                <h3 data-num="1">{{open[1]? '-': '+'}}</h3>
            </div>
        </div>
        <div class="answer" v-if="open[1]">
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odio ea ipsa molestias illum dolor laboriosam dolorum obcaecati magnam minus nisi. Atque porro veritatis neque magni in autem amet a, vitae aliquid doloremque deleniti cumque, perspiciatis consectetur mollitia deserunt facilis, sequi hic nobis voluptatem nemo labore quam? Amet veniam repellendus aliquid.</p>
        </div>
    </div>
    <div class="contain">
        <div :class="['community' ,open[2]?'active':'']">
            <h6>who Lorem ipsum dolor sit amet consectetur?</h6>
            <div class="button" @click="change">
                <h3 data-num="2">{{open[2]? '-': '+'}}</h3>
            </div>
        </div>
        <div class="answer" v-if="open[2]">
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odio ea ipsa molestias illum dolor laboriosam dolorum obcaecati magnam minus nisi. Atque porro veritatis neque magni in autem amet a, vitae aliquid doloremque deleniti cumque, perspiciatis consectetur mollitia deserunt facilis, sequi hic nobis voluptatem nemo labore quam? Amet veniam repellendus aliquid.</p>
        </div>
    </div>
    <div class="contain">
        <div :class="['community' ,open[3]?'active':'']">
            <h6>who Lorem ipsum dolor sit amet consectetur?</h6>
            <div class="button" @click="change">
                <h3 data-num="3">{{open[3]? '-': '+'}}</h3>
            </div>
        </div>
        <div class="answer" v-if="open[3]">
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odio ea ipsa molestias illum dolor laboriosam dolorum obcaecati magnam minus nisi. Atque porro veritatis neque magni in autem amet a, vitae aliquid doloremque deleniti cumque, perspiciatis consectetur mollitia deserunt facilis, sequi hic nobis voluptatem nemo labore quam? Amet veniam repellendus aliquid.</p>
        </div>
    </div>
</div>
</template>





<script>
export default{
    data(){
        return{
            open:[true , false , false , false]
        }
    },
    methods:{
        change:function(e){
            let num = e.target.getAttribute('data-num')
            if(this.open[num]){
                return this.open[num] = false
            }
            for(let i=0 ; i<this.open.length ; i++){
                this.open[i]=false
            }
            this.open[num]  = true
        }
    }
}
</script>

<style scoped>
.contain{
    border-bottom: 1px solid #00000048;
    padding: 0%;
    margin: 0;
}
.community{
    position: relative;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0%;
    margin: 0%;
    
}
.active,
.community{
    transition: .3s;
}
.active{
    color: var(--main-color);
}
.community .button{
    background-color: #fff;
    width: 20px;
    height: 20px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}
.community .button:hover{
    cursor:default;
}
</style>