<template>
  <!-- <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel" target="_blank" rel="noopener">babel</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-router" target="_blank" rel="noopener">router</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-vuex" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">eslint</a></li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">vue-devtools</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">awesome-vue</a></li>
    </ul>
  </div> -->
  <header class="header">
    <div class='header__logo'>
      <Logo />
    </div>
    <div class="header__burger-menu">
      <BurgerMenu />
    </div>
    <nav class="header__nav">
      <ul class="header__nav-links">
        <li class="header__nav-link">
          <a href="#">Пункт 1</a>
        </li>
        <li class="header__nav-link">
          <a href="#">Пункт 2</a>
        </li>
        <li class="header__nav-link">
          <a href="#">Пункт 3</a>
        </li>
        <li class="header__nav-link">
          <a href="#">Пункт 4</a>
        </li>
      </ul>
    </nav>
    <div class="header__contacts">
      <a href="tel:+7 (999) 111-11-11" class="header__phone">+7 (999) 111-11-11</a>
    </div>
  </header>
</template>

<script>
import Logo from '@/components/Logo.vue'
import BurgerMenu from '@/components/BurgerMenu.vue'

export default {
  name: 'Header',
  components: {
    Logo,
    BurgerMenu
  }
  // ,
  // props: {
  //   msg: String
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .header{
    display: flex;
    height: 96px;
    width: 100%;
    padding: 0 64px;
    align-items: center;
    &__burger-menu {
      padding: 0 19px;
    }
    &__nav {
      border-bottom: 2px solid;
      border-image-source: linear-gradient(270deg,
       rgba(255, 255, 255, 0) -1.08%,
       rgba(255, 255, 255, 0.15) 44.88%,
       rgba(255, 255, 255, 0) 97.05%);
      border-image-slice: 1;
      flex-grow: 100;
      height: calc(100% - 40px);
      margin: 0 64px;
      &-links {
        height: 100%;
        padding: 0;
        margin: 0;
        display: flex;
        align-items: center;
        justify-content: center;
        list-style-type: none;
      }
      &-link {
        & a {
          display: flex;
          align-items: center;
          font-style: normal;
          font-weight: bold;
          font-size: 14px;
          line-height: 25px;
          color: #FFFFFF;
          opacity: 0.7;
          margin-right: 49px;
          &:hover {
            opacity: 1;
            &::before {
              visibility: visible;
            }
          }
          &::before {
            visibility: hidden;
            content: "";
            display: block;
            width: 7px;
            height: 7px;
            background: linear-gradient(180deg, #EE7374 0%, #FC664F 100%);
            border-radius: 50%;
            margin-right: 7px;
          }
        }
      }
    }
    &__phone {
      font-style: normal;
      font-weight: bold;
      font-size: 14px;
      line-height: 40px;
      color: #FFFFFF;
      opacity: 0.7;
      &:hover{
        opacity: 1;
      }
    }
  }
</style>
