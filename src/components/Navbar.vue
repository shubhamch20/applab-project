<template>
  <div class="logo-header">
    <div class="desktop">
      <div class="logo-wrapper">
        <div class="logo-wrapper-top-section" style="cursor:pointer">
          <span class="app-logo-text">App</span>
          <span class="lab-logo-text">Lab</span>
        </div>
        <div class="nav-section">
          <div class="custom-nav-text">Home</div>
          <div class="custom-nav-text">Key Features</div>
          <div class="custom-nav-text">Pricing</div>
          <div class="custom-nav-text">Testiminial</div>
          <div class="custom-nav-text">FAQ</div>
          <b-button pill>Try for free</b-button>
        </div>
      </div>
    </div>
    <div class="mobile-nav">
      <b-sidebar id="sidebar-1" shadow>
        <div class="logo-wrapper-top-section " style="cursor:pointer">
          <span class="app-logo-text">App</span>
          <span class="lab-logo-text">Lab</span>
        </div>
        <div class="custom-nav-mob-text">Home</div>
        <div class="custom-nav-mob-text">Key Features</div>
        <div class="custom-nav-mob-text">Pricing</div>
        <div class="custom-nav-mob-text">Testiminial</div>
        <div class="custom-nav-mob-text">FAQ</div>
        <b-button style="margin-top: 10px" pill>Try for free</b-button>
      </b-sidebar>
    </div>
    <b-button class="mob-side" v-b-toggle.sidebar-1>☰</b-button>
  </div>
</template>


<script>
export default {
  name: "logo-header",
  mixins: [],
  data() {
    return {
      drawer: false,
    };
  },
  created() {
    // console.log(this.fromRecoPage);
  },
  methods: {
    OpenNavBtn() {
      this.drawer = true;
    },
  },
};
</script>


<style  scoped>
.mob-side {
  display: none;
}

.logo-wrapper {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.app-logo-text {
  font-size: 28px;
  font-weight: 600;
  color: orange;
}
.lab-logo-text {
  color: #242f51;
  font-size: 28px;
  font-weight: 600;
}
.nav-section {
  align-items: center;
  display: flex;
}
.custom-nav-mob-text {
  padding: 18px 40px;
  font-size: 1rem;
  color: #000;
  transition: 0.3s;
  text-align: left;
  border-bottom: 1px solid #b5b5b5;
  cursor: pointer;
}
.btn-secondary {
  padding: 0.375rem 1.32rem;
  color: #fff;
  background-color: #2563ff;
}
.logo-wrapper {
  padding: 40px 25px;
}

.custom-nav-text {
  margin-right: 20px;
  color: #242f51;
  cursor: pointer;
  font-size: 16px;
  font-family: "Poppins", sans-serif;
}
.custom-nav-text:hover {
  cursor: pointer;
  text-decoration: underline;
  text-shadow: 0 0 black;
}
@media screen and (max-width: 700px) {
  .desktop {
    display: none;
  }
  .mob-side {
    display: block;
    background-color: transparent;
    color: black;
    border: none;
    font-size: 30px;
  }
}

</style>
<style>
.btn-secondary:not(:disabled):not(.disabled):active,
.btn-secondary:not(:disabled):not(.disabled).active,
.show > .btn-secondary.dropdown-toggle {
  background-color: transparent !important;
  color: #000 !important;
}
@media screen and (max-width: 550px) {
  .b-sidebar:not(.b-sidebar-right) {
    width: 100% !important;
  }
}
</style>