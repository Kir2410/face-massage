<template>
    <footer>
        <div class="up"></div>
        <div class="down"></div>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="sass" scoped>
@import '@/styles/variables.sass'

footer
    position: fixed
    bottom: 0
    right: 0
    left: 0

.up
    height: 430px
    width: 100%
    background: $line
    
.down
    height: 140px
    width: 100%
    background: $text-dark
</style>