<template>
  <HeaderComponent/>
  <main>Contents goes here</main>
  <FooterComponent/>
</template>

<script>
import FooterComponent from './components/FooterComponents.vue';
import HeaderComponent from './components/HeaderComponent.vue';
export default {
  components: {
    HeaderComponent,
    FooterComponent
}
}
</script>

<style lang="scss" scoped>

</style>