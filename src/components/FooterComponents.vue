<template>
    <footer >
        <div class="top-footer">
            <div class="container"></div>
        </div>
        <div class="bottom-footer">
            <div class="container"></div>
        </div>
    </footer>
</template>

<script>
    export default {
    name: "FooterComponent",
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
    .top-footer {
        background-image: url('../assets/img/footer-bg.jpg'); 
        background-size: cover;
        height: 300px;
    }
    .bottom-footer {
        background-color: $darkgray;
    }
</style>