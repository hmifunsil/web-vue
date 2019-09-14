<template>
      <div class="md-layout">
        <div class="md-layout-item md-size-50 md-small-size-100 from-us">
            <img
            :src="tentang"
            alt="Raised Image"
            class="img-raised rounded"
            :class="{ 'responsive-image': responsive }"
          />
          <h1>Tentang HMIF</h1>
          <h2>Pelajari tentang himpunan mahasiswa informatika</h2>
          <a href="#/tentang">Lebih lanjut</a>
        </div>
            
        <div class="md-layout-item md-size-50 md-small-size-100 from-us"><img
            :src="akademik"
            alt="Raised Image"
            class="img-raised rounded"
            :class="{ 'responsive-image': responsive }"
          />
          
          <h1>Akademik</h1>
          <h2>Pelajari apa saja mata kuliah di jurusan informatika unsil</h2>
          <a href="#">Lebih lanjut</a></div>
        <div class="md-layout-item md-size-50 md-small-size-100 from-us"><img
            :src="komunitas"
            alt="Raised Image"
            class="img-raised rounded"
            :class="{ 'responsive-image': responsive }"
          />
          
          <h1>Komunitas</h1>
          <h2>Pelajari tentang komunitas di jurusan informatika</h2>
          <a href="#">Lebih lanjut</a></div>
        <div class="md-layout-item md-size-50 md-small-size-100 from-us"><img
            :src="event"
            alt="Raised Image"
            class="img-raised rounded"
            :class="{ 'responsive-image': responsive }"
          />
          
          <h1>Event</h1>
          <h2>Lihat event terbaru kami</h2>
          <a href="#">Lebih lanjut</a></div>
      </div>
</template>

<script>

export default {
  components: {
  },
  data() {
    return {
      tentang: require("@/assets/img/Tentang.png"),
      akademik: require("@/assets/img/Akademik.png"),
      event: require("@/assets/img/Event.png"),
      komunitas: require('@/assets/img/komunitas.jpg'),
      responsive: false
    };
  },
};
</script>

<style lang="css"></style>