<template>
    <div class="menu">
        <button class="menu__btn">
            <span class="menu__btn-detail-1"></span>
            <span class="menu__btn-detail-2"></span>
            <span class="menu__btn-detail-3"></span>
        </button>
    </div>
</template>

<script>
export default {
  name: 'BurgerMenu'
}
</script>

<style scoped lang="scss">
    .menu {
        &__btn {
            width: 23.81px;
            display: flex;
            padding: 0;
            margin: 0;
            border: 0;
            background: none;
            cursor: pointer;
            height: 18px;
            outline: none;
            flex-direction: column;
            justify-content: space-between;
            &-detail-1,
            &-detail-2,
            &-detail-3 {
                width: 100%;
                height: 2px;
                background-color: #fff;
                opacity: 0.7;
                border-radius: 1.5px;
            }
            &:hover &-detail-1,
            &:hover &-detail-2,
            &:hover &-detail-3{
                opacity: 1;
            }
        }
    }
</style>
