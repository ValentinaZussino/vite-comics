<template>
    <div id="blue-bar">
        <div class="container">
            <div v-for="(link, index) in linksImages" :key="index" class="icon">
                <img :src="getImagePath(`../assets/img/${link.url}`)" class="img-icon">
                <a href="#">{{link.text}}</a>
            </div>
        </div> 
    </div>
</template>

<script>
    export default {
        name: 'BluebarComponent',
        data(){
            return {
                linksImages : [
                    {
                        text: 'digital comics',
                        url: 'buy-comics-digital-comics.png'
                    },
                    {
                        text: 'dc merchandise',
                        url: 'buy-comics-merchandise.png'
                    },
                    {
                        text: 'subscription',
                        url: 'buy-comics-subscriptions.png'
                    },
                    {
                        text: 'comic shop locator',
                        url: 'buy-comics-shop-locator.png'
                    },
                    {
                        text: 'dc power visa',
                        url: 'buy-dc-power-visa.svg'
                    }
                ]
            }
        },
        methods: {
            getImagePath(imgPath){
                return new URL(imgPath, import.meta.url).href;
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
    #blue-bar{
        background-color: $blue;

        .container {
            justify-content: center;
		    align-items: center;
            .icon{
            display: flex;
			justify-content: center;
			align-items: center;
            flex-basis: calc(100% - 10rem) / 5;
            padding: 1rem;
            .img-icon{
                width: 45px;
                margin-right: 10px;
            }
            &:nth-child(4) .img-icon { width: 28px; padding-right: 0;}
            a{
                color: white;
                font-size: 15px;
                font-weight: 400;
                text-transform: uppercase;
                text-decoration: none;
            }
        }
        }
    }
</style>