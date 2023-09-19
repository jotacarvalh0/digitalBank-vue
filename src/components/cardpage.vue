<template>
    <section class="container-project">
        <div class="container-card">
            <cardstart/>
        </div>

        <div class="container-image">
            <img src="../../public/img-cred-card.png" alt="">
        </div>
    </section>
</template>

<script>
import cardstart from '../components/cardstart.vue'

    export default {
        name: 'CardPage',
        components: {
            cardstart,

        }
    }
</script>

<style lang="sass">
$color1: #131213
$color2: #2C2C2C
$white: #F5F5F5

//card
$pink: #DD45C5
$bluec: #354668
$cardd: $bluec, $pink, $bluec

@mixin gradient($direction, $cardd) 
  background: -webkit-linear-gradient($direction, $cardd)

body
    background-color: $color1
    margin: 0
    padding: 0
    box-sizing: border-box
    font-family: Arial, Helvetica, sans-serif

    .container-project
        display: flex
        justify-content: center
        margin: 0 auto
        height: 700px
        
        .container-image
            width: 50%
            display: flex
            justify-content: center
            align-items: center
            img
                margin: 0 auto
                width: 500px

</style>