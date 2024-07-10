<template>
  <footer>
        <div class="logo">
            <img src="../assets/img/mirketgiller_logo_white.png" alt="mirketgiller">
        </div>
        <div class="linkItem">
            <div class="quickLinks">
              <h2>Hızlı Bağlantılar</h2>
              <div class="links">
                <router-link to="/">Düzenlediğimiz Etkinlikler</router-link>
                <router-link to="/">Blog</router-link>
                <router-link to="/">Galeri</router-link>
                <router-link to="/">SSS</router-link>
              </div>
            </div>
            <div class="whoUs">
              <h2>Mirketgiller</h2>
              <div class="links">
                <router-link to="/">Biz Kimiz?</router-link>
                <router-link to="/">Ekibimiz</router-link>
              </div>
            </div>
            <div class="contact">
              <h2>İletişim</h2>
              <div class="links">
                  <router-link to="" class="mail"><i class="bi bi-envelope"></i>iletişim@mirketgiller.com
                  </router-link>
                
                <div class="contactLinks">
                  <a href="https://www.linkedin.com/company/mirketgiller/mycompany/verification/"><i class="bi bi-linkedin"></i></a>
                  <a href="https://www.instagram.com/mirketgiller_/"><i class="bi bi-instagram"></i></a>
                  <a href="https://www.youtube.com/@mirketgiller"><i class="bi bi-youtube"></i></a>
                  <a href="https://x.com/mirketgiller"><i class="bi bi-twitter-x"></i></a>

                </div>
              </div>
            </div>
        </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style>
a{
  color: white;
  font-size: 20px;
}
footer{
    width: 100%;
    height: 281px;
    display: flex;
    padding: 60px;
    gap: 120px;
    background-color: #D37C26;
    color: #FFFFFF;
}
.logo img{
  width: 254px;
  height: auto;
}
.linkItem{
  width: 100%;
  display: flex;
  align-items: start;
  justify-content: center;
  flex-direction: row;
  gap: 60px;
  color: white;
}
.linkItem h2{
  font-size: 24px;
  padding-bottom: 4px;
  font-weight: bold;
}
.mail{
  display: flex;
  gap: 10px;
}
footer a.router-link-exact-active{
  color: #FFFFFF;
  font-size: 16px;
}
footer a.router-link-exact-active:hover{
  transition: .2s ease all;
  text-decoration: underline;
}
.links{
  display: flex;
  flex-direction: column;
  gap: 10px;
  font-size: 20px;
}
.contact .mail{
  display: flex;
  gap: 10px;
}
.contactLinks{
  display: flex;
  flex-direction: row;
  gap: 10px;
}

@media (max-width: 1169px) {
  footer{
    gap: 38px;
}
.links{
  gap: 2px;
}
.linkItem{
  gap: 18px;
}
  footer a.router-link-exact-active{
    color: #FFFFFF;
    font-size: 16px;
  }
  .linkItem h2{
    font-size: 20px;
  }
}
@media (max-width: 988px) {
  footer{
    gap: 20px
  }
  .linkItem{
    gap:12px;
  }
  .links{
    font-size: 16px;
    gap: 8px;
  }
}
@media (max-width: 969px) {
  footer{
    flex-direction: column;
    height: auto;
    align-items: center;
    padding: 40px;
    gap: 80px;
  }
  .logo img{
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .linkItem{
    gap: 20px;
  }
  .links{
    font-size: 14px;
    gap: 20px;
  }
  .linkItem h2{
    font-size: 22px;
  }
}

@media (max-width: 648px) {
  footer{
    flex-basis: 180px;
  }
  .links{
    font-size: 12px;
    gap: 2px;
  }
  .linkItem{
    flex-direction: column;
  }
  .linkItem h2{
    font-size: 18px;
  }
}
</style>