<template>
    <footer >
        <div class="top-footer">
            <div class="container">
                <div class="col">
                    <span>dc comics</span>
                    <ul>
                        <li v-for="(link, index) in linksComics" :key="index">
                            <a href="#">{{link.text}}</a>
                        </li>
                    </ul>
                    <span>shop</span>
                    <ul>
                        <li v-for="(shop, index) in linksShop" :key="index">
                            <a href="#">{{shop.text}}</a>
                        </li>
                    </ul>
                </div>
                <div class="col"></div>
                <div class="col"></div>
            </div>
        </div>
        <div class="bottom-footer">
            <div class="container"></div>
        </div>
    </footer>
</template>

<script>
    export default {
    name: "FooterComponent",
    data(){
            return {
                linksComics: [
                    {
                        text: "Characters",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Comics",
                        url: "#",
                        current: true,
                    },
                    {
                        text: "Movies",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "TV",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Games",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Collectibles",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Videos",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Fans",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "News",
                        url: "#",
                        current: false,
                    },
                ],
                linksShop: [
                    {
                        text: "Shop DC",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Shop DC Collectibles",
                        url: "#",
                        current: false,
                    },
                ]
            }
        }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
    .top-footer {
        background-image: url('../assets/img/footer-bg.jpg'); 
        background-size: cover;
        min-height: 300px;

        .col {
            // width: 100px;
            margin-right: 20px;
            border: 1px solid red;

            span{text-transform: uppercase; color: white;}
            ul{ 
                list-style: none;
                padding-top: 13px;
                li{
                    padding-bottom: 5px;
                    a{text-decoration: none; color: $lightgray; font-size: 13px;}
                }
            }
        }
    }
    .bottom-footer {
        background-color: $darkgray;
    }
</style>