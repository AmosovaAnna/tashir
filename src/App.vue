<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

html, body{
  padding: 0;
  margin: 0;
  width: 1920px;
  height: 1079px;
  overflow: hidden;
  & *{
    box-sizing: border-box;
    font-family: 'Montserrat', sans-serif;
    transition: .2s;
  }
}
a{
  text-decoration: none;
}
#app{
  height: 100%;
}
</style>
