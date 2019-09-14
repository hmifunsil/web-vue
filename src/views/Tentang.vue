<template>
  <div class="wrapper">
    <parallax
      class="section page-header header-filter"
      :style="headerStyle"
    ></parallax>
    <div class="main tentang-content">
      <div class="section ">
        <div class="container">
          <div class="md-layout">
              <img
            :src='require("@/assets/img/head-tentang.png")'
            alt="Raised Image"
            class="img-raised"
            :class="{ 'responsive-image': responsive }"
          />
          <div class="tentang-title">
              <h2>TENTANG</h2>
              <h1>HIMPUNAN</h1>
              <h1>MAHASISWA INFORMATIKA</h1>
              <h1>UNIVERSITAS SILIWANGI</h1>
          </div>
          <div class="tentang-konten">
              <h5>DESKRIPSI HMIF</h5>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
              </p>
              <h5>STUKTUR KEPENGURUSAN</h5>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur illo aspernatur maxime quis quo sapiente? Odio cupiditate voluptas quisquam, optio aut veritatis corrupti laudantium facilis, reprehenderit totam laboriosam blanditiis distinctio.
              </p>
          </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { Tabs } from "@/components";
export default {
  components: {
  },
  bodyClass: "profile-page",
  data() {
    return {
    };
  },
  props: {
    header: {
      type: String,
      default: require("@/assets/img/Jumbotron.png")
    },
    img: {
      type: String,
      default: require("@/assets/img/faces/christian.jpg")
    }
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`,
      };
    }
  }
};
</script>

<style lang="scss" scoped>
.section {
  padding: 0;
}

.profile-tabs /deep/ {
  .md-card-tabs .md-list {
    justify-content: center;
  }

  [class*="tab-pane-"] {
    margin-top: 3.213rem;
    padding-bottom: 50px;

    img {
      margin-bottom: 2.142rem;
    }
  }
}
</style>
