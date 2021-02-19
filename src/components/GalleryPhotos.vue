<template>
    <div class="gallery">
        <ul class="gallery__photos">
            <li v-on:click="$emit('openPhoto', car.src); selectPhoto(car)" v-for="car in cars" class="gallery__photo" v-bind:class="{gallery__photo_active: car.select}" v-bind:key="car.id">
              <img v-bind:src="car.src" alt="Машина">
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'GalleryPhotos',
  data: function () {
    return {
      cars: [
        {
          select: true,
          id: 1,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/1164906.jpg'
        },
        {
          select: false,
          id: 2,
          src: 'https://s0.rbk.ru/v6_top_pics/resized/1440xH/media/img/0/64/755546152905640.jpg'
        },
        {
          select: false,
          id: 3,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/mash2.jpg'
        },
        {
          select: false,
          id: 4,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/mash3.jpg'
        },
        {
          select: false,
          id: 5,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/1164907.jpg'
        },
        {
          select: false,
          id: 6,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/maxresdefault-9.jpg'
        },
        {
          select: false,
          id: 7,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/Samy-e-krasivy-e-mashiny-foto.jpg'
        },
        {
          select: false,
          id: 8,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/ssc-tuatara1.jpg'
        },
        {
          select: false,
          id: 9,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/92830063_0031-2.jpg'
        },
        {
          select: false,
          id: 10,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/1469788208143851659.jpg'
        },
        {
          select: false,
          id: 11,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/foto11.jpg'
        },
        {
          select: false,
          id: 12,
          src: 'https://bipbap.ru/wp-content/uploads/2017/09/1-1.jpg'
        }
      ]
    }
  },
  methods: {
    selectPhoto: function (car) {
      for (const obj of this.cars) {
        for (const key in obj) {
          if (key === 'select') {
            obj[key] = false
          }
        }
      }
      car.select = true
    }
  }
}
</script>

<style scoped lang="scss">
  .gallery {
    padding: 20px 64px;
    &__photos {
      list-style-type: none;
      padding: 0;
      display: flex;
      justify-content: space-between;
      margin: 0 -10px;
    }
    &__photo {
      width: calc(125.62px + 20px);
      height: calc(125.62px + 20px);
      overflow: hidden;
      cursor: pointer;
      filter: drop-shadow(0px 4px 30px rgba(0, 0, 0, 0.25));
      border-radius: 20px;
      opacity: 0.6;
      display: flex;
      align-items: center;
      justify-content: center;
      img {
        object-fit: cover;
        width: calc(100% - 20px);
        height: calc(100% - 20px);
        border-radius: 20px;
      }
      &_active,
      &:hover,
      &:focus,
      &:active {
        opacity: 1;
        background: linear-gradient(180deg, #EF7674 0%, #EF8865 100%);
      }
    }
  }
</style>
