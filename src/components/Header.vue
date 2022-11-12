<template>
    <header>
        <div class="logo">
            <img src="@/assets/logo.png" alt="" class="logo-image">
            <div class="logo-arrow">
                <span>&#9660</span>
            </div>
        </div>
        <nav class="navbar">
            <span>О нас</span>
            <span>Массаж</span>
            <span>Масла</span>
            <span>Акции</span>
            <span>Контакты</span>
        </nav>
        <div class="user-panel">
            <div class="user-panel__wrapper">

            </div>
            <span>rus</span>
            <img src="@/assets/icons/Search.svg" alt="">
            <img src="@/assets/icons/Bag-icon.svg" alt="">
        </div>
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style lang="sass" scoped>
@import '@/styles/variables.sass'

header
    position: fixed
    top: 0
    right: 0
    left: 0
    display: flex
    align-items: center
    justify-content: space-between
    height: 90px
    background: $background

.logo
    display: flex
    align-items: center
    justify-content: space-between
    height: 100%
    width: 20%
    &-image
        height: 100%
        //width: 60%
    &-arrow
        display: flex
        align-items: center
        justify-content: center
        height: 100%
        width: 30%
        border-left: 1px solid $line
        border-right: 1px solid $line
        cursor: pointer

.navbar
    & span
        text-transform: uppercase
        font-size: 12px
        color: $text
        cursor: pointer
        &:not(:last-child)
            margin-right: 42px
        &:hover
            color: $text-dark

.user-panel
    display: flex
    align-items: center
    justify-content: space-between
    padding: 0 5%
    height: 100%
    width: 20%
    border-top: 20px solid $primary
    border-bottom: 20px solid $primary
    & span
        text-transform: uppercase
        font-size: 12px
        color: $text-middle
</style>