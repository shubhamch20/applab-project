<template>
  <div class="Footer">
      <div class="footer-top-section" style="cursor:pointer">
        <span class="app-logo-text">App</span>
        <span class="lab-logo-text">Lab</span>
      </div>
      <div class="footer-section">
        <div class="custom-nav-text">Home</div>
        <div class="custom-nav-text">Key Features</div>
        <div class="custom-nav-text">Pricing</div>
        <div class="custom-nav-text">Testiminial</div>
        <div class="custom-nav-text">FAQ</div>
    </div>
    <div class="social-icon">
      <img src="../assets/Facebook100px.png" alt="" height="23px" width="23px">
      <img src="../assets/Twitter100px.png" alt="" height="23px" width="23px">
      <img src="../assets/Instagram100px.png" alt="" height="23px" width="23px">
    </div>
  </div>
</template>


<script>
export default {
  name: "Footer",
  mixins: [],
  data() {
    return {};
  },
  created() {
    // console.log(this.fromRecoPage);
  },
  methods: {
   
  },
};
</script>


<style  scoped>

.app-logo-text {
  font-size: 28px;
  font-weight: 600;
  color: orange;
}
.social-icon{
  display: flex;
  justify-content: center;
  margin-top: 20px;
}
.social-icon img{
  margin: 10px 30px 10px 0px;
    filter: brightness(16) invert(1);
}
.footer-top-section{
text-align: center;
}
.Footer{
  padding: 50px 25px 70px;
  background-color:#242f51 ;
}
.lab-logo-text {
  color: #FFF;
  font-size: 28px;
  font-weight: 600;
}
.footer-section {
  align-items: center;
  display: flex;
  justify-content: center;
  margin-top: 10px;
  flex-wrap: wrap;
}


.custom-nav-text {
  /* margin-right: 20px; */
  color: #FFF;
  font-size: 16px;
  font-family: "Poppins", sans-serif;
  margin: 8px 20px 0;
  cursor: pointer;
}
.custom-nav-text:hover {
    cursor: pointer;
    text-decoration: underline;
}
@media screen and (max-width: 600px) {
}
</style>