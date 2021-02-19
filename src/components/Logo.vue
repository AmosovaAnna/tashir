<template>
    <div class="logo">
        <a class="logo__link" href="#">
            <div class="logo__icon"></div>
        </a>
    </div>
</template>

<script>
export default {
  name: 'Logo'
}
</script>

<style scoped lang="scss">
  .logo {
    &__link {
      display: block;
      padding: 10px;
    }
    &__icon {
      display: block;
      border-radius: 50%;
      width: 36px;
      height: 36px;
      box-shadow: 0px -20px 10px 15px #ef8865, 0px 10px 10px 15px #ef7674;
      -webkit-clip-path: circle(28px);
      clip-path: circle(28px);
    }
  }
</style>
