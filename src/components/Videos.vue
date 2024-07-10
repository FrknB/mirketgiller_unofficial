<template>
  <div class="videoBox">
    <div class="title">
        <h1>Videolar</h1>
    </div>
    <div class="videoArea">
        <iframe src="https://www.youtube.com/embed/ZmTtzYC8qiY?si=od6J2zQGHkfHzdlU" poster="../assets/img/mirketgiller_logo.png"></iframe >
        <iframe src="https://www.youtube.com/embed/ZmTtzYC8qiY?si=od6J2zQGHkfHzdlU" poster="../assets/img/mirketgiller_logo.png"></iframe >
        <iframe src="https://www.youtube.com/embed/ZmTtzYC8qiY?si=od6J2zQGHkfHzdlU" poster="../assets/img/mirketgiller_logo.png"></iframe >
    </div>

    <div class="more">
        <a target="_blank" href="https://www.youtube.com/channel/UCw4toFAgNQ6UO0w9yu4ND8w">Youtube Sayfamıza Göz Atın</a>
    </div>
    
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.title{
    text-align: center;
    font-weight: bold;
    width: 100%;
    font-size: 40px;
    color: #FFFFFF;
    margin-bottom: 40px;
}
.videoBox{
    width: 100%;
    height: 517px;
    margin-top: 80px;
    padding: 60px 80px;
    background-color: #1C1C1C;
}
.videoArea{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    flex-basis: 200px;
    gap: 30px;
}
.videoArea iframe{
    width: 350px;
    height: 196px;
    border-radius: 12px;
    border: 1px solid #808080;
    margin-bottom: 40px;
}
.more{
    width: 100%;
    text-align: center;
    display: flex;
    justify-content: center;
}
.more a{
    font-size: 20px;
    color: #A0A0A0;
    width: auto;
    border-bottom: 2px solid #D37C26;
    transition: .3s all ease;
    cursor: pointer;
}
.more a:hover{
    color: #FFFFFF;
}
@media (max-width: 1221px) {
    .videoBox{
        height: auto;
        padding: 60px 60px;
    }
}
@media (max-width: 475px) {
    .videoBox{
        padding: 60px 20px;
    }
    .more a{
        font-size: 14px;
    }
}
@media (max-width: 391px) {
    .videoBox{
        padding: 40px 0;
    }
    .more a{
        font-size: 18px;
    }
    .videoArea iframe{
        width: 300px;
        height: 166px;
    }
}
@media (max-width: 326px) {
    .videoBox{
        margin: 0;
    }
}
</style>