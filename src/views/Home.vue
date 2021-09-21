<template>
  <div class="home">
    <Navbar></Navbar>
    <div class="modern-app-section">
      <div class="modern-app-main">
        <div class="modern-app-top-text1">#1 Editiors Choice App of 2020</div>
        <div class="modern-app-top-text2">
          Best app for your modern lifestyle
        </div>
        <div class="modern-app-top-text3">
          Increase productivity with a single-to-do app for managing your
          personal budgets
        </div>
        <div class="watch-demo">
          <b-button pill>Try for free</b-button>
          <div style="cursor:pointer;color:#2563ff">Watch demo video</div>
        </div>
      </div>
      <div class="mobile-img">
        <img src="../assets/phone.png" alt="" />
      </div>
    </div>
    <div class="company-section">
      <div class="trusted-company-text">Trusted by companies like</div>
      <div class="company-logo">
        <img class="custom-logo" src="../assets/southwest.png" alt="" />
        <img class="custom-logo" src="../assets/anubis.png" alt="" />
        <img class="custom-logo" src="../assets/alonzo.png" alt="" />
        <img class="custom-logo" src="../assets/express.png" alt="" />
        <img class="custom-logo" src="../assets/maniac.png" alt="" />
      </div>
    </div>
    <div class="apps-featres-sec">
      <div class="smart-search">
        <img src="../assets/smart-search.png" alt="" />
      </div>
      <div class="app-features-texts">
        <div class="modern-app-top-text2">Awesome apps features</div>
        <div class="modern-app-top-text3" style="margin-bottom: 50px">
          Increase productivity with a single-to-do app for managing your
          personal budgets
        </div>
        <div class="img-details-app-features">
          <div class="custom-img-bg" style="background-color: #efbaba">
            <img src="../assets/speed.png" alt="" width="50px" height="50px" />
          </div>
          <div>
            <div style="color:#f55767;">Fast Performance</div>
            <div class="img-details-text">
              Get your blood delivered at home collect a sample from the news
              your blood tests.
            </div>
          </div>
        </div>
        <div class="img-details-app-features">
          <div class="custom-img-bg" style="background-color: #e8e4e4">
            <img
              src="../assets/prototyping.png"
              alt=""
              width="50px"
              height="50px"
            />
          </div>
          <div>
            <div style="color:#2563ff;">Prototyping</div>
            <div class="img-details-text">
              Get your blood delivered at home collect a sample from the news
              your blood tests.
            </div>
          </div>
        </div>
        <div class="img-details-app-features">
          <div class="custom-img-bg" style="background-color: #7ddea0">
            <img
              src="../assets/vector-editing.png"
              alt=""
              width="50px"
              height="50px"
            />
          </div>
          <div>
            <div style="color:#40975f;">Vector Editing</div>
            <div class="img-details-text">
              Get your blood delivered at home collect a sample from the news
              your blood tests.
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import Footer from "../components/Footer";
import Navbar from "../components/Navbar.vue";
export default {
  name: "Home",
  components: {
    Navbar,
    Footer,
  },
};
</script>
<style scoped>
.modern-app-top-text3 {
  color: #242f51;
  width: 390px;
  font-size: 16px;
  font-family: "Poppins", sans-serif;
  margin-bottom: 15px;
}
.custom-img-bg {
  display: flex;
  justify-content: center;
  height: 75px;
  width: 75px;
  align-items: center;
  border-radius: 50%;
}

.custom-logo {
  width: 120px;
  height: 40px;
  margin: 8px 20px;
}
.company-logo {
  margin-bottom: 65px;
  margin-top: 20px;
  align-items: center;
  display: flex;
  justify-content: center;
}
.smart-search img {
  height: 660px;
}
.smart-search {
  background-image: url("../assets/smart-search-bg.png");
  background-repeat: no-repeat;
  background-position: bottom;
  background-size: 100%;
}
.img-details-text {
  color: #242f51;
  width: 260px;
  font-size: 16px;
  font-family: "Poppins", sans-serif;
}
.apps-featres-sec {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}
.trusted-company-text {
  color: #242f51;
  font-size: 16px;
  font-family: "Poppins", sans-serif;
}
.watch-demo {
  align-items: center;
  display: flex;
  justify-content: space-between;
  width: 282px;
}
.mobile-img img {
  height: 660px;
}
.img-details-app-features {
  margin-bottom: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.app-features-texts {
  text-align: left;
}
.btn-secondary {
  padding: 0.375rem 1.32rem;
  color: #fff;
  background-color: #2563ff;
}
.modern-app-main {
  text-align: left;
}
.modern-app-section {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  background-image:url("../assets/hero-vector.png"), url("../assets/skyline.png") ;
  
  background-repeat: no-repeat, no-repeat;
  background-position:top, bottom  ;
  background-size: 100% 250% , 100%;
}
.modern-app-top-text2 {
  color: #242f51;
  font-size: 28px;
  width: 250px;
  font-weight: 600;
  font-family: "Poppins", sans-serif;
}
.modern-app-top-text1 {
  color: #242f51;
  width: 270px;
  text-align: center;
  background-color: #eaead8;
  font-size: 15px;
  border-radius: 10px;
  font-weight: 600;
  font-family: "Poppins", sans-serif;
}
.company-section {
  margin-top: 40px;
}
@media screen and (max-width: 900px) {
  .mobile-img img {
    height: 500px;
  }
  .smart-search img {
    height: 500px;
  }
  .apps-featres-sec {
    flex-direction: column;
  }
}
@media screen and (max-width: 750px) {
  .modern-app-section {
    flex-direction: column;
  background-size: contain;

  }
  .company-logo {
    flex-wrap: wrap;
    justify-content: space-evenly;
  }

}
@media screen and (max-width: 550px) {
  .modern-app-top-text3 {
    width: 90%;
  }
  .modern-app-top-text2 {
    width: 90%;
  }
  /* .modern-app-top-text1{
    width: 90%;
  } */
  .img-details-text {
    width: 100%;
  }
  .custom-img-bg {
    margin: 8px 0;
  }
  .app-features-texts {
    padding: 25px;
  }
  .modern-app-main {
    padding: 25px;
  }
  .img-details-app-features {
    flex-direction: column;
    align-items: unset
    ;
  }
}
@media screen and (max-width: 430px) {
  .mobile-img img {
    height: 400px;
  }
  .smart-search img {
    height: 400px;
  }
}
</style>
