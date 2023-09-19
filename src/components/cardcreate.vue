<template>
    <h1>teste</h1>
</template>

<script>
    export default {
        name: 'CardCreate',
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

.container-card
    display: flex
    flex-direction: column
    justify-content: center
    align-items: center
    width: 50%
    margin-top: 4rem
    margin-left: 30p
    color: $white
    .card
        @include gradient(left, $cardd)
        width: 400px
        height: 250px
        border-radius: 30px
        .start-card-info
            .balance
                font-size: 40px
                color: $white
                padding-left: 30px
                p
                    font-size: 20px
                    margin: 0
                    margin-top: 2rem
                h1
                    margin: 0
            .card-info
                display: flex
                align-items: flex-end
                padding-left: 30px
                gap: 1.5rem
                margin-top: 4.2rem
                .card-flag
                    svg
                        color: $white
                        width: 50px
                        height: 36px
                .card-name
                    color: $white
</style>