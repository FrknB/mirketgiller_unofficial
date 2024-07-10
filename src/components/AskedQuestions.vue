<template>
  <div class="askedQuestions">
    <div class="title">
        Sıkça Sorulan Sorular
    </div>
        <div class="textBox"  v-for="question in questions" :key="question">
            <div class="questionTitle">
                <h2 :class="{titleActive: question.show }" @click="toggleButton(question)">{{ question.title }}<i :class="[changeIcon(question), {iconActive: question.show}]"></i></h2>
            </div>
            <div :class="['desc', {active: question.show}]" v-if="question.show">
                <span>{{ question.desc }}</span>
            </div>
        </div>

  </div>
</template>

<script>
export default {
    data() {
        return {
            slide: false,
            questions: [
                {
                    show: false,
                    title: "1.kutu",
                    desc: "kfdljajgkha alkdf jgkla jkagfjk fdlşbgkflkdjgklfadjhkljafdk lhjklafdjhkgljafdklhjalkfdjhkla fdjhglkjafdlkhjakfldjhlkadjkhajfkdlgjakl jkagf jkagfj kfagj kl ajgkfajgklşjgf aşkljakljklgjkajkljkglf"
                },
                {
                    show: false,
                    title: "2.kutu",
                    desc: "kfdljajgkha alkdf jgkla jkagfjk ajfkdlgjakl jkagf jkagfj kfagj kl ajgkfajgklşjgf aşkljakljklgjkajkljkglf"
                },
                {
                    show: false,
                    title: "3.kutu",
                    desc: "kfdljajgkha alkdf jgkla jkagfjk ajfkdlgjakl jkagf jkagfj kfagj kl ajgkfajgklşjgf aşkljakljklgjkajkljkglf"
                }
            ]
        }
    },
    computed:{
        changeIcon(){
            return (question) => question.show ? 'bi bi-caret-up-fill' :'bi bi-caret-down';
        },
    },
    methods: {
        toggleButton(question){
            question.show =! question.show;
        }
    },
}
</script>

<style scoped>
.askedQuestions{
    width: 100%;
    height: auto;
    padding: 60px 80px;
    background-color: #1C1C1C;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}
.title{
    color: #FFFFFF;
    text-align: center;
    font-weight: bold;
    font-size: 40px;
    margin-bottom: 40px;
    transition: .3s ease;
}
.textBox{
    width: 80%;
    background-color: #202020;
    border-radius: 16px;
    margin-bottom: 12px;
    transition: .4s ease;
}
.textBox .questionTitle{
    font-size: 20px;
    padding: 24px 16px;
    transition: .3s ease;
    color: white;
}
.questionTitle h2{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0;
    cursor: pointer;
    transition: .3s ease;
}
.titleActive{
    color: #D37C26;
}
.questionTitle i{
    transition: 1s ease all;
    transform: translate(0deg);
}
.iconActive{
    transform: rotate(360deg);
}
.desc{
    height: auto;
    background-color: #303030;
    color: #A0A0A0;
    font-size: 20px;
    padding: 24px 16px;
    transition: 1s ease all;
    opacity: 0;
    height: 0%;
}
.desc span{
    padding: 0 10px;
    overflow-wrap: break-word;
}
.active{
    opacity: 1;
    height: 100%;
    border-radius: 0 0 16px 16px;
}

@media (max-width: 1150px) {
    .askedQuestions{
        height: auto;
        padding: 60px 60px;
    }
}
@media (max-width: 530px) {
    .askedQuestions{
        height: auto;
        padding: 60px 20px;
    }
    .desc{
        font-size: 14px;
    }
}
@media (max-width: 340px) {
    .title{
        font-size: 28px;
    }
    .desc{
        font-size: 12px;
    }
}
</style>