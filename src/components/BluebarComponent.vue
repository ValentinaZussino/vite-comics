<template>
    <div id="blue-bar">
        <div class="container">
            Blue bar
        </div> 
    </div>
</template>

<script>
    export default {
        name: 'BluebarComponent',
        data(){
            return {
                linksImage : [
                    {
                        text: 'digital comics',
                        url: '../assets/img/buy-comics-digital-comics.png'
                    },
                    {
                        text: 'dc merchandise',
                        url: '../assets/img/buy-comics-merchandise.png'
                    },
                    {
                        text: 'subscription',
                        url: '../assets/img/buy-comics-subscriptions.png'
                    },
                    {
                        text: 'comic shop locator',
                        url: '../assets/img/buy-comics-shop-locator.png'
                    },
                    {
                        text: 'dc power visa',
                        url: '../assets/img/buy-dc-power-visa.svg'
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
    #blue-bar{
        background-color: $blue;
    }
</style>