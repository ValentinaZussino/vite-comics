<template>
    <header>
        <div class="container container-header">
            <a href="#" id="top-logo">
                <img src="../assets/img/dc-logo.png" alt="DC logo">
            </a>
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index" :class="{'active': link.current}">
                        <a :href="link.url" :class="{'active': link.current}">{{link.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data(){
            return {
                links: [
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
                    {
                        text: "Shop",
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
    header {
        .container-header {
            justify-content: space-between;
            align-items: center;
            height: 80px;
        }
        #top-logo {width: 60px}
        nav {height: 80px;}
        ul {
            height: 100%;
            list-style: none;
            display: flex;
            justify-content: center;
            align-items: center;
            
            li {
                height: 100%;
                a {
                display: inline-block;
                text-decoration: none;
                font-weight: 600;
                font-size: 13px;
                text-transform: uppercase;
                color: $darkgray;
                padding: 0 1rem;
                line-height: 80px;
                &.active {
                    color: $blue;
                }
                }
                &:hover {background-color: rgb(221, 221, 221);}
                &.active {
                    border-bottom: 3px solid $blue;
                }
            }
            
        }
    }
</style>