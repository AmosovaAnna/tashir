<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <div class="container-background">
      <div class="container-background__1"></div>
      <div class="container-background__2"></div>
      <div class="container-background__3"></div>
    </div>
    <Header />
    <GalleryPhotos v-on:openPhoto="openPhoto" />
    <div class="main-content">
      <InfoCar />
      <GalleryPhotoShow :srcPhoto="srcChosenPhoto" />
    </div>
  </div>
</template>
<style scoped lang="scss">
  .home{
    height: 100%;
    position: relative;
  }
  .container-background{
    z-index: -1;
    height: 100%;
    width: 100%;
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
    position: absolute;
    background: linear-gradient(13deg, #212121 69.8%, #8D3D32 95.15%);
    & .container-background__1{
      background: linear-gradient(284.64deg, rgba(103, 14, 0, 0.7) -0.29%, rgba(117, 21, 6, 0.7) -1.23%, rgba(99, 20, 7, 0.7) 30.64%, rgba(0, 0, 0, 0.7) 66.38%);
      -webkit-backdrop-filter: blur(40px);
      backdrop-filter: blur(40px);
      height: 100%;
      width: 100%;
      position: absolute;
      filter: blur(5px);
    }
    & .container-background__3{
      background: linear-gradient(2.57deg, #0F0F0F -5.97%, rgba(46, 9, 3, 0.21) 52.49%), linear-gradient(230.31deg, rgba(252, 101, 77, 0) 77.31%, #FC654D 100.38%);
      transform: rotate(-180deg);
      height: 100%;
      width: 100%;
      position: absolute;
      filter: blur(2px);
    }
    & .container-background__2{
      background: radial-gradient(50% 50% at 50% 50%, #FC654D 25%, rgba(252, 101, 77, 0) 100%);
      position: absolute;
      width: 1497px;
      height: 1497px;
      right: -50%;
      top: -35%;
      filter: blur(2px);
    }
  }
  .main-content {
    display: flex;
    flex-grow: 1;
    height: 100%;
  }
</style>

<script>
import Header from '@/components/Header.vue'
import GalleryPhotos from '@/components/GalleryPhotos.vue'
import GalleryPhotoShow from '@/components/GalleryPhotoShow.vue'
import InfoCar from '@/components/InfoCar.vue'

export default {
  name: 'Home',
  components: {
    Header,
    GalleryPhotos,
    GalleryPhotoShow,
    InfoCar
  },
  data: function () {
    return {
      srcChosenPhoto: 'https://bipbap.ru/wp-content/uploads/2017/09/1164906.jpg'
    }
  },
  methods: {
    openPhoto: function (src) {
      this.srcChosenPhoto = src
    }
  }
}
</script>
