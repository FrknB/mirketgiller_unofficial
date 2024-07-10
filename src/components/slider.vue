<template>
  <div class="sliderBox">
    <div id="carouselExampleIndicators" class="carousel slide">
        <div class="carousel-indicators">
          <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
          <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
          <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="../assets/img/header-background.png" class="d-block w-100" alt="#">
          </div>
          <div class="carousel-item">
            <img src="../assets/img/header-background.png" class="d-block w-100" alt="#">
          </div>
          <div class="carousel-item">
            <img src="../assets/img/header-background.png" class="d-block w-100" alt="#">
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.sliderBox{
  width: 100%;
  height: auto;
    margin: 0 auto;
    padding: 80px 20px 0 20px ;
    background-color: #202020;
    display: flex;
    align-items: center;
    justify-content: center;
}

@media (max-width: 400px) {
  .sliderBox{
    display: none;
  }
  
}
</style>