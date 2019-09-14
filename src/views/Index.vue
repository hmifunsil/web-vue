<template>
  <div class="wrapper">
    <parallax class="page-header header-filter" :style="headerStyle">
      <div class="md-layout">
        <div class="md-layout-item">
          <div class="image-wrapper">
            <div class="brand">
              <h2>Halaman Resmi</h2>
              <h1>Himpunan Mahasiswa</h1>
              <br>
              <h1>Informatika</h1>
              <h3>Universitas Siliwangi</h3>
              <div class="header-horizontal"></div>
            </div>
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised">
      <div class="section section-basic" >
        <div class="container">
          <div class="title">
            <h2>Dari Kami</h2>
            <dari-kami></dari-kami>
          </div>
        </div>
      </div>
      <div class="section section-akademik" :style="{ backgroundImage: 'url(' + require('@/assets/img/Jumbotron2.png') + ')' }">
        <div class="container">
          <div class="title">
            <h2>Akademik</h2>
            <akademik></akademik>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import DariKami from './components/DariKamiSection';
import Akademik from './components/AkademikSection';

export default {
  components: {
    DariKami,
    Akademik
  },
  name: "index",
  bodyClass: "index-page",
  props: {
    image: {
      type: String,
      default: require("@/assets/img/Jumbotron.png")
    },
    signup: {
      type: String,
      default: require("@/assets/img/city.jpg")
    },
    landing: {
      type: String,
      default: require("@/assets/img/landing.jpg")
    },
    profile: {
      type: String,
      default: require("@/assets/img/profile.jpg")
    }
  },
  data() {
    return {};
  },
  methods: {
    leafActive() {
      if (window.innerWidth < 768) {
        this.leafShow = false;
      } else {
        this.leafShow = true;
      }
    }
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.image})`
      };
    },
    signupImage() {
      return {
        backgroundImage: `url(${this.signup})`
      };
    }
  },
  mounted() {
    this.leafActive();
    window.addEventListener("resize", this.leafActive);
  },
  beforeDestroy() {
    window.removeEventListener("resize", this.leafActive);
  }
};
</script>
<style lang="scss">
.section-download {
  .md-button + .md-button {
    margin-left: 5px;
  }
}

@media all and (min-width: 991px) {
  .btn-container {
    display: flex;
  }
}
</style>
