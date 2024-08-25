<template>
  <header>
    <div class="logo">
      <router-link to="/" class="active"
        ><img src="../assets/img/mirketgiller_logo.png" alt=""
      /></router-link>
    </div>
    <nav>
      <ul class="nav-links" :class="{ navActive: isActive }">
        <router-link to="/" class="active"><li>Biz Kimiz?</li></router-link>
        <router-link to="/"><li>Düzenlediğimiz Etkinlikler</li></router-link>
        <router-link to="/"><li>Ekibimiz</li></router-link>
        <router-link to="/"><li>Blog</li></router-link>
        <router-link to="/"><li>Galeri</li></router-link>
      </ul>
      <div class="burger">
        <i class="bi bi-list" @click="toggleClass"></i>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    toggleClass() {
      this.isActive = !this.isActive;
    },
  },
};
</script>

<style scoped>
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  padding: 40px 80px 0px 80px;
}
header img {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 36px;
}
nav {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 40px;
  font-size: 20px;
}
.nav-links {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 40px;
  position: relative;
  transition: 0.5s all ease-in;
}
.nav-links a.router-link-exact-active {
  color: #f2f2f2;
  font-size: 20px;
  transition: 0.2s ease all;
}
.nav-links a.router-link-exact-active:hover {
  color: #d37c26;
}

.burger {
  width: 40px;
  height: 40px;
  display: none;
  align-items: center;
  justify-content: center;
}
.burger i {
  cursor: pointer;
  font-size: 36px;
  color: #f2f2f2;
}

@media (max-width: 1100px) {
  .burger {
    display: flex;
  }
  .nav-links {
    display: none;
  }

  .navActive {
    transition: .5s ease all;
    display: flex;
    position: absolute;
    flex-direction: column;
    top: 100px;
    z-index: 5;
    right: 0;
    width: 100%;
    height: 100%;
    padding: 60px 60px;
    border-radius: 12px 0 0 12px;
    gap: 60px;
    background-color: #202020;
    transition: 0.5s ease all;
    border: 1px solid #f1f1f1;
    background: url("../assets/img/header-background.png");
  }
  .navActive a.router-link-exact-active {
    display: flex;
    align-items: center;
    justify-content: center;
    border-bottom: 1px solid #d37c26;
  }
  .navActive a.router-link-exact-active:hover {
    display: flex;
    align-items: center;
    justify-content: center;
    border-bottom: 1px solid #f2f2f2;
  }
}
@media (max-width: 500px) {
  header{
    width: 100%;
  padding: 40px;
  }
  .navActive {
    width: 100%;
    height: 100%;
  }
}
@media (max-width: 326px) {
  header{
    width: 100%;
  padding: 40px 20px;
  }
  .navActive {
    width: 100%;
    height: 100vh;
  }
  .navActive a.router-link-exact-active{
    font-size: 16px;
  }
}
</style>