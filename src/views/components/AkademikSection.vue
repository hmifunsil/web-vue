<template>
      <div class="md-layout">
        <div class="md-layout-item md-size-50 md-small-size-100 from-us">
            <img
            :src="alumni"
            alt="Raised Image"
            class="img-raised rounded"
            :class="{ 'responsive-image': responsive }"
          />
          <h1>Alumni</h1>
          <h2>Lihat tentang alumni</h2>
          <a href="#">Lebih lanjut</a>
        </div>
            
        <div class="md-layout-item md-size-50 md-small-size-100 from-us"><img
            :src="jurnal"
            alt="Raised Image"
            class="img-raised rounded"
            :class="{ 'responsive-image': responsive }"
          />
          
          <h1>Jurnal</h1>
          <h2>Lihat jurnal di jurusan Informatika unsil</h2>
          <a href="https://journal.unsil.ac.id/home" target="_blank">Lebih lanjut</a></div>
      </div>
</template>

<script>

export default {
  components: {
  },
  data() {
    return {
      jurnal: require("@/assets/img/jurnal.jpg"),
      alumni: require("@/assets/img/Alumni.png"),
      responsive: false
    };
  },
};
</script>

<style lang="css"></style>