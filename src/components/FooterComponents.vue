<template>
    
    <footer >
        <div class="top-footer">
            <div class="container">
                <div class="wrapper-col">
                    <div class="col">
                        <span>dc comics</span>
                        <ul>
                            <li v-for="(link, index) in linksComics" :key="index">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                        <span>shop</span>
                        <ul>
                            <li v-for="(link, index) in linksShop" :key="index">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col">
                        <span>dc</span>
                        <ul>
                            <li v-for="(link, index) in linksDc" :key="index">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col">
                        <span>sites</span>
                        <ul>
                            <li v-for="(link, index) in linksSites" :key="index">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div id="dc-bground">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="bottom-footer">
            <div class="container">
                <button>sign-up now!</button>
                <div>
                    <span>follow us</span>
                    <a><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
                    <a><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
                    <a><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
                    <a><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
                    <a><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
                </div>
            </div>
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
                ],
                linksDc: [
                    {
                        text: "Terms Of Use",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Privacy Policy (New)",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Add Choices",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Advertising",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Jobs",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Subscriptions",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Talent Workshops",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "CPSC Certificates",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Ratings",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Shop Help",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "Contacts Us",
                        url: "#",
                        current: false,
                    },
                ],
                linksSites: [
                    {
                        text: "DC",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "MAD Magazine",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "DC Kids",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "DC Universe",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "DC Power Visa",
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
        .container {
            padding: 0 2rem;
            justify-content: space-between;
            .wrapper-col {
                display: flex;
                .col {
                    margin-right: 20px;

                    span{text-transform: uppercase; color: white; display: inline-block; margin-top: 2rem;}
                    ul{ 
                        list-style: none;
                        padding-top: 12px;
                        li{
                            padding-bottom: 5px;
                            a{text-decoration: none; color: $lightgray; font-size: 13px;}
                        }
                        li:last-of-type{
                            padding-bottom: 20px;
                        }
                    }
                }
            }
            #dc-bground {
                height: 500px;
                overflow: hidden;
                margin-top: -70px;
            }
        }
        
    }
    .bottom-footer {
        background-color: $darkgray;
        div.container {
            justify-content: space-between;
            align-items: center;

            button {
            background-color: transparent;
            border: 2px solid $blue;
            color: white;
            text-transform: uppercase;
            padding: 15px;
            }

            > div {
                display: flex;
                justify-content: center;
                align-items: center;
                span {
                text-transform: uppercase;
                color: $blue;
                font-weight: bold;
                padding-right: 20px;
                }
                a {padding-right: 0.8rem; 
                    img {
                        width:30px;
                        cursor: pointer;
                    }   
                }
            }
        }
        
    }
</style>