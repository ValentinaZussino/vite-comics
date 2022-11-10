<template>
    <header>
        <a href="#">
            <img src="../assets/img/dc-logo.png" alt="DC logo">
        </a>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </nav>
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

</style>