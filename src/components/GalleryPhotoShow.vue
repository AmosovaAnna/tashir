<template>
    <div ref="containerPhoto" v-bind:class="{animationOn: animationOn}" class="photoShow">
        <div class="photoShow__background"></div>
        <div class="photoShow__container-for-bacgkrounds-circles circle">
          <div class="circle__1">
            <div ref="circle" class="circle__2">
              <svg width="668" height="668" viewBox="0 0 668 668" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M334.082 660.595C261.942 660.595 191.832 636.704 134.704 592.654C77.5747 548.603 36.6415 486.873 18.2992 417.103C-0.0430332 347.334 5.23614 273.455 33.3121 207.002C61.3899 140.55 110.683 85.2671 173.495 49.7867C236.308 14.308 309.103 0.627805 380.509 10.8857C451.916 21.1436 517.916 54.76 568.202 106.488C618.486 158.214 650.224 225.137 658.46 296.805C666.697 368.474 650.966 440.852 613.725 502.637" stroke="url(#paint0_linear1)" stroke-width="13.906" stroke-linecap="round"/>
              <defs>
              <linearGradient id="paint0_linear1" x1="334.082" y1="7.56758" x2="334.082" y2="660.595" gradientUnits="userSpaceOnUse">
              <stop stop-color="#EF7674"/>
              <stop offset="0.963542" stop-color="#EF8766"/>
              </linearGradient>
              </defs>
              </svg>
            </div>
            <div class="circle__3">
              <div ref="detail1" class="circle__3-detail-1">
                <svg width="327" height="653" viewBox="0 0 327 653" fill="none" xmlns="http://www.w3.org/2000/svg">
                <g opacity="0.7">
                <mask id="path-1-inside-1-1" fill="white">
                <path d="M0.17557 0.0754862C42.9998 0.0754844 85.4046 8.51036 124.969 24.8984C164.533 41.2865 200.483 65.307 230.764 95.5882C261.045 125.87 285.066 161.819 301.454 201.383C317.842 240.947 326.277 283.352 326.277 326.176C326.277 369.001 317.842 411.406 301.454 450.97C285.066 490.534 261.045 526.483 230.764 556.765C200.483 587.046 164.533 611.066 124.969 627.455C85.4046 643.843 42.9998 652.278 0.175568 652.278L0.175584 326.176L0.17557 0.0754862Z"/>
                </mask>
                <path d="M0.17557 0.0754862C42.9998 0.0754844 85.4046 8.51036 124.969 24.8984C164.533 41.2865 200.483 65.307 230.764 95.5882C261.045 125.87 285.066 161.819 301.454 201.383C317.842 240.947 326.277 283.352 326.277 326.176C326.277 369.001 317.842 411.406 301.454 450.97C285.066 490.534 261.045 526.483 230.764 556.765C200.483 587.046 164.533 611.066 124.969 627.455C85.4046 643.843 42.9998 652.278 0.175568 652.278L0.175584 326.176L0.17557 0.0754862Z" stroke="url(#paint0_linear2)" stroke-opacity="0.8" stroke-width="280" mask="url(#path-1-inside-1-1)"/>
                </g>
                <defs>
                <linearGradient id="paint0_linear2" x1="228.034" y1="121.435" x2="-20.0509" y2="452.489" gradientUnits="userSpaceOnUse">
                <stop stop-color="#FC654D"/>
                <stop offset="0.5" stop-color="#FC654D" stop-opacity="0.5"/>
                <stop offset="1" stop-color="#FC654D" stop-opacity="0"/>
                </linearGradient>
                </defs>
                </svg>
              </div>
              <div ref="detail2" class="circle__3-detail-2">
                <svg width="693" height="662" viewBox="0 0 693 662" fill="none" xmlns="http://www.w3.org/2000/svg">
                <g opacity="0.7">
                <mask id="path-1-inside-1-2" fill="white">
                <path d="M461.765 0.588241C492.046 30.8695 516.066 66.8186 532.455 106.383C548.843 145.947 557.277 188.352 557.278 231.176C557.277 274.001 548.843 316.406 532.455 355.97C516.066 395.534 492.046 431.483 461.765 461.765C431.483 492.046 395.534 516.066 355.97 532.455C316.406 548.843 274.001 557.278 231.176 557.277C188.352 557.278 145.947 548.843 106.383 532.455C66.8186 516.066 30.8695 492.046 0.588232 461.765L231.176 231.176L461.765 0.588241Z"/>
                </mask>
                <path d="M461.765 0.588241C492.046 30.8695 516.066 66.8186 532.455 106.383C548.843 145.947 557.277 188.352 557.278 231.176C557.277 274.001 548.843 316.406 532.455 355.97C516.066 395.534 492.046 431.483 461.765 461.765C431.483 492.046 395.534 516.066 355.97 532.455C316.406 548.843 274.001 557.278 231.176 557.277C188.352 557.278 145.947 548.843 106.383 532.455C66.8186 516.066 30.8695 492.046 0.588232 461.765L231.176 231.176L461.765 0.588241Z" stroke="url(#paint0_linear3)" stroke-opacity="0.8" stroke-width="280" mask="url(#path-1-inside-1-2)"/>
                </g>
                <defs>
                <linearGradient id="paint0_linear3" x1="537.071" y1="247.522" x2="127.558" y2="306.191" gradientUnits="userSpaceOnUse">
                <stop stop-color="#FC654D"/>
                <stop offset="0.5" stop-color="#FC654D" stop-opacity="0.5"/>
                <stop offset="1" stop-color="#FC654D" stop-opacity="0"/>
                </linearGradient>
                </defs>
                </svg>
              </div>
              <div class="photoShow__photo">
                <img ref="mainPhotoCar" v-bind:src="srcChosenPhoto" alt="Машина">
              </div>
            </div>
          </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'GalleryPhotoShow',
  props: ['srcPhoto'],
  data: function () {
    return {
      srcChosenPhoto: 'https://bipbap.ru/wp-content/uploads/2017/09/1164906.jpg',
      animationOn: false
    }
  },
  watch: {
    srcPhoto: function () {
      const context = this
      // this.$refs.mainPhotoCar.style = 'visibility: hidden'
      this.$nextTick(() => {
        this.animationOn = true
        this.srcChosenPhoto = this.srcPhoto
        this.$refs.mainPhotoCar.onload = function () {
          setTimeout(function () {
            // context.$refs.mainPhotoCar.style = 'visibility: visible'
            context.animationOn = false
          }, 300)
        }
      })
    }
  }
}
</script>

<style scoped lang="scss">
  .photoShow {
    position: relative;
    height: 100%;
    flex-grow: 1;
    justify-content: center;
    display: flex;
    overflow: hidden;
    &__background {
      background: radial-gradient(50% 50% at 50% 50%, #FC654D 0%, rgba(252, 101, 77, 0) 100%);
      position: absolute;
      top: 0;
      width: 841.26px;
      height: 841.26px;
      left: calc(60% - (841.26px / 2));
    }
    &__photo {
      border-radius: 50%;
      z-index: 1;
      overflow: hidden;
      width: 554px;
      height: 554px;
      filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
      margin-top: -93px;
      margin-left: -93px;
      img {
        object-fit: cover;
        width: 100%;
        height: 100%;
      }
    }
    &__container-for-bacgkrounds-circles{
      width: 715.78px;
      height: 709.99px;
      border-radius: 50%;
      border: 5px solid rgba(255, 129, 129, 0.25);
      justify-content: center;
      display: flex;
      align-items: center;
      & .circle__1{
        width: 640.35px;
        height: 640.35px;
        background: linear-gradient(194.45deg, #D8D8D8 17.13%, rgba(216, 216, 216, 0) 95.91%);
        border-radius: 50%;
        position: relative;
      }
      & .circle__2{
        position: absolute;
        top: -13.91px;
        left: -13.91px;
      }
      & .circle__3{
        border: 137px solid rgba(255, 255, 255, 0.2);
        border-radius: 50%;
        height: 100%;
        width: 100%;
        position: relative;
        &-detail-1{
          position: absolute;
          top: -145px;
          left: -145px;
          opacity: 0.7;
          width: 652.02px;
          height: 652.02px;
          display: flex;
          justify-content: flex-end;
        }
        &-detail-2{
          position: absolute;
          top: -140px;
          left: -140px;
          opacity: 0.7;
          width: 652.02px;
          height: 652.02px;
          display: flex;
          justify-content: flex-end;
          svg {
            width: 327px;
            height: 653px;
            transform: scale(2.165) translate(-23.5px, 42px);
          }
        }
      }
    }
    &.animationOn{
      .circle__2,
      .circle__3-detail-1,
      .circle__3-detail-2{
        animation-iteration-count: infinite;
        animation: rotate360 .28s linear;
      }
      .circle__3-detail-2{
        animation: rotate360 .25s linear;
      }
      .circle__2{
        animation: rotate360 .3s linear;
      }
    }
  }
  @keyframes rotate360 {
    from {
      transform: rotate(0);
    }
    25%{
      transform: rotate(90deg);
    }
    50%{
      transform: rotate(180deg);
    }
    75%{
      transform: rotate(270deg);
    }
    to {
      transform: rotate(360deg);
    }
  }
</style>
