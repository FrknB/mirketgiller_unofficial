<template>
  <div class="whatThisEvent">
        <div class="title">
            <h1>Nedir Bu Etkinlikler ?</h1>
            <p>Mirketgiller ekibi olarak durmaksızın etkinlikler düzenliyoruz. Kurulduğumuz günden bugüne, öğrencilerin kendilerini<br>geliştirebilmeleri için, çeşitli alanlarda <span style="color: #D37C26;">webinarlar, zirveler ve online atölyeler</span> düzenledik.</p>
        </div>
        <div class="cards">
            <div class="cardItem">
                <div class="icon"><i class="bi bi-youtube"></i></div>
                <div class="cardtitle">Webinarlar</div>
                <div class="desc">
                    Mirketgiller ekibi olarak, öğrencilerin kendilerini geliştirmeleri için, alanında uzman kişileri öğrenciler ile online ortamda buluşturuyoruz.
                </div>
            </div>
            <div class="cardItem">
                <div class="icon"><i class="bi bi-buildings"></i></div>
                <div class="cardtitle">Zirveler</div>
                <div class="desc">
                    Mirketgiller ekibi olarak, öğrencilerin kendilerini geliştirmeleri için, alanında uzman kişileri öğrenciler ile yüzyüze ortamda buluşturuyoruz.
                </div>
            </div>
            <div class="cardItem">
                <div class="icon"><i class="bi bi-mortarboard"></i></div>
                <div class="cardtitle">Online Atölyeler</div>
                <div class="desc">
                    Mirketgiller ekibi olarak, öğrencilerin kendilerini geliştirmeleri için, alanında uzman kişileri öğrenciler ile online ortamda buluşturuyoruz ve eğitimler veriyoruz.
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped> 
.whatThisEvent{
    width: 100%;
    height: 680px;
    display: flex;
    flex-direction: column;
    padding: 60px 80px;
    gap: 60px;
}
.title{
    width: 100%;
    height: auto;
    display: flex;
    flex-direction: column;
    justify-content: start;
    text-align: center;
    border: none;
    gap: 24px;
}
.title h1{
    color: #FFFFFF;
    font-size: 40px;
}
.title p{
    color: #A0A0A0;
    font-size: 20px;
}
.cards{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 30px;
}
.cardItem{
    display: flex;
    flex-direction: column;
    height: 60px;
    width: 350px;
    height: 368px;
    border-radius: 16px;
    padding: 24px;
    background-color: #1C1C1C;
    color: #FFFFFF;
}
.cardItem .icon{
    font-size: 60px;
}
.cardItem .cardtitle{
    font-size: 32px;
    font-weight: bold;
    color: #D37C26;
    text-align: left;
    margin-bottom: 12px;
}
@media (max-width: 1150px) {
    .whatThisEvent{
        height: auto;
        padding: 60px 60px;
    }
    .cards{
        flex-wrap: wrap;
    }
    .title h1{
        font-size: 38px;
    }
}
@media (max-width: 540px) {
    .title h1{
        font-size: 30px;
    }
    .title p{
        font-size: 16px;
    }
    .whatThisEvent{
        height: auto;
        padding: 20px;
    }
    .cardItem{
        height: 400px;
    }
}
@media (max-width: 340px) {
    .title h1{
        font-size: 27px;
    }
}
</style>