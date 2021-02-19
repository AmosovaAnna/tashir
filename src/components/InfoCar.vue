<template>
    <div class="infoCar">
        <ul class="infoCar__list">
            <li class="infoCar__section" v-bind:class="{open: info.open}" v-for="info of infoList" v-bind:key="info.id">
              <h2 class="infoCar__header">{{ info.title }}</h2>
              <p class="infoCar__text">{{ info.content }}</p>
              <ul class="infoCar__addresses">
                <li class="infoCar__address" v-for="address of info.adresses" v-bind:key="address.id">
                  <div class="infoCar__address-icon">
                    <img :src="address.img" alt="">
                  </div>
                  <div class="infoCar__address-text">{{address.address}}</div>
                </li>
              </ul>
              <img class="infoCar__img" :src="info.img" alt="Статистика">
              <div @click="openInfo(info)" class="infoCar__openSection">
                <svg width="11" height="23" viewBox="0 0 11 23" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path opacity="0.7" fill-rule="evenodd" clip-rule="evenodd" d="M4.53969 16.1718C7.40356 13.8285 7.40356 9.44955 4.53969 7.1062L0.773146 4.02425C-0.143524 3.27419 -0.143524 1.87257 0.773146 1.12251C1.46373 0.557448 2.45689 0.557449 3.14748 1.12251L7.59061 4.75808C11.938 8.31535 11.938 14.9627 7.5906 18.52L3.14748 22.1555C2.45689 22.7206 1.46373 22.7206 0.773146 22.1555C-0.143524 21.4055 -0.143524 20.0039 0.773146 19.2538L4.53969 16.1718Z" fill="#D9D9D9"/>
                </svg>
              </div>
            </li>
        </ul>
    </div>
</template>

<script>
// import func from '../../vue-temp/vue-editor-bridge'
export default {
  name: 'infoCar',
  data: function () {
    return {
      infoList: [
        {
          id: 1,
          open: true,
          title: 'Характеристики авто',
          content: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu.',
          adresses: [
            {
              id: 11,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'м. Новые Черемушки'
            },
            {
              id: 12,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 13,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 14,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 15,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            }
          ],
          img: 'https://techrocks.ru/wp-content/uploads/2020/01/The-Noun-Project-min.png'
        },
        {
          id: 2,
          open: false,
          title: 'Цена',
          content: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu.',
          adresses: [
            {
              id: 21,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'м. Новые Черемушки'
            },
            {
              id: 22,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 23,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 24,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 25,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            }
          ],
          img: 'https://techrocks.ru/wp-content/uploads/2020/01/The-Noun-Project-min.png'
        },
        {
          id: 3,
          open: false,
          title: 'Интерьер',
          content: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu.',
          adresses: [
            {
              id: 31,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'м. Новые Черемушки'
            },
            {
              id: 32,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 33,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 34,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 35,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            }
          ],
          img: 'https://techrocks.ru/wp-content/uploads/2020/01/The-Noun-Project-min.png'
        },
        {
          id: 4,
          open: false,
          title: 'Экстерьер',
          content: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu.',
          adresses: [
            {
              id: 41,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'м. Новые Черемушки'
            },
            {
              id: 42,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 43,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 44,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            },
            {
              id: 45,
              img: 'https://img.icons8.com/ios/452/job.png',
              address: 'Xxxxxxxx xxxxxxxx'
            }
          ],
          img: 'https://techrocks.ru/wp-content/uploads/2020/01/The-Noun-Project-min.png'
        }
      ]
    }
  },
  methods: {
    openInfo: function (elem) {
      for (const obj of this.infoList) {
        for (const key in obj) {
          if (key === 'open') {
            obj[key] = false
          }
        }
      }
      elem.open = true
    }
  }
}
</script>

<style scoped lang="scss">
  .infoCar{
    &__list{
      max-width: 620px;
      width: 100%;
      padding: 0;
      margin: 0;
      display: flex;
      overflow: hidden;
      list-style-type: none;
      height: 801px;
    }
    &__section{
      width: 45px;
      color: white;
      overflow: hidden;
      background: linear-gradient(182.91deg, #0D0B0B 4.31%, #303030 50.78%, #0B0A0A 94.29%);
      box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.25);
      position: relative;
      &.open{
        // padding: 10px 30px 20px 60px;
        width: 485px;
        .infoCar__text,
        .infoCar__addresses,
        .infoCar__img{
          transform: none;
          visibility: visible;
        }
        .infoCar__header {
          writing-mode: horizontal-tb;
          transform: none;
          font-style: normal;
          font-weight: bold;
          font-size: 32px;
          line-height: 25px;
          color: #E7E7E7;
          margin: 10px 30px 6px 60px;
        }
        .infoCar__openSection{
          transform: rotate(-180deg);
          pointer-events: none;
          opacity: 0.2;
          right: 15px;
        }
      }
    }
    &__header {
      margin: 0;
      writing-mode: vertical-lr;
      // transform: rotate(-180deg);
      transform: scale(-1, -1);
    }
    &__text{
      transform: translateX(-15vw);
      font-style: normal;
      font-weight: 600;
      font-size: 12px;
      line-height: 20px;
      width: 355px;
      margin: 10px 30px 30px 60px;
      visibility: hidden;
    }
    &__addresses{
      transform: translateX(-15vw);
      padding: 0;
      margin: 0;
      list-style-type: none;
      width: 355px;
      margin: 10px 30px 20px 60px;
      visibility: hidden;
    }
    &__address{
      display: flex;
      align-items: center;
      margin-bottom: 15px;
      &-icon{
        width: 40px;
        height: 40px;
        margin-right: 20px;
        & > *{
          width: 100%;
          height: 100%;
          object-fit: contain;
        }
      }
    }
    &__img{
      width: 100%;
      transform: translateX(-15vw);
      width: 355px;
      margin: 20px 30px 0 60px;
      visibility: hidden;
    }
    &__openSection{
      position: absolute;
      bottom: 0;
      right: 0;
      opacity: 0.7;
      border-radius: 30px;
      width: 45px;
      height: 55px;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
    }
  }
</style>
