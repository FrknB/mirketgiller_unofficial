<template>
  <div class="homeArea">
    <div class="homeItem">
      <h1 class="title">Birlikte Büyüyen<br />Yetenekler</h1>
      <p class="description">
        Bizler gönüllü olarak etkinlikler ve webinarlar düzenleyen,<br />
        birbirimizle etkileşim halinde olan
        <span style="font-weight: bold">Mirketgiller</span>’iz.
      </p>
      <div class="buttonArea">
        <router-link to="/" class="buttons"
          ><i class="bi bi-people"></i>Topluluğumuza Katıl</router-link
        >
        <router-link to="/" class="buttons"
          ><i class="bi bi-person-plus"></i>Ekibimize Katıl</router-link
        >
      </div>
    </div>
    <div class="eventBox">
      <div class="boxItem">
        <h2>3500+</h2>
        <span>Kişiye ulaştık</span>
      </div>
      <div class="boxItem">
        <h2>15+</h2>
        <span>Etkinlik yaptık</span>
      </div>
      <div class="boxItem">
        <h2>310+</h2>
        <span>İş birliğine ortak olduk</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.homeArea {
  width: 100%;
  height: 588px;
  position: relative;
  padding: 0 80px;
}
.homeItem {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  flex-wrap: wrap;
  color: #a0a0a0;
  gap: 40px;
  text-align: center;
}
.title {
  color: #f1f1f1;
  font-size: 52px;
}
.buttonArea {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 16px;
}
.buttons {
  border-radius: 24px;
  padding: 16px 20px;
  color: white;
  background-color: #d37c26;
  display: flex;
  gap: 10px;
}
.buttons:hover {
  background-color: #ac6015;
  transition: 0.3s all ease;
}
.eventBox {
  height: 137px;
  position: absolute;
  bottom: -52px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
  width: 90%;
  z-index: 4;
  padding: 0 80px;
}
.boxItem {
  background-color: #1a1a1a;
  border-radius: 16px;
  width: 350px;
  height: 137px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 8px;
}
.boxItem h2 {
  color: #d37c26;
}
.boxItem span {
  color: #a0a0a0;
}

@media (max-width: 768px) {
  .homeArea {
    height: auto;
    padding: 0 0 40px 0;
  }
  .eventBox {
    display: none;
  }
  .title {
    font-size: 42px;
  }
  .description{
    font-size: 14px;
  }
  .buttons {
    padding: 16px 20px;
    gap: 10px;
  }
}
@media (max-width: 612px) {
  .buttonArea {
    flex-wrap: wrap;
  }
}
@media (max-width: 530px) {
  .title {
    font-size: 34px;
  }
  .description{
    font-size: 12px;
  }
  .homeItem {
    gap: 20px;
  }
  .buttonArea {
    flex-wrap: wrap;
  }
}
@media (max-width: 326px) {
  .homeArea{
    padding: 0 20px 40px 20px;
  }
  .title {
    font-size: 34px;
  }
  .description{
    font-size: 12px;
  }
}
</style>