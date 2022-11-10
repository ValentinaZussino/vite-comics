<template>
    <div id="blue-bar">
        <div class="container">
            Blue bar
        </div> 
    </div>
</template>

<script>
    export default {
        name: 'BluebarComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
    #blue-bar{
        background-color: $blue;
    }
</style>