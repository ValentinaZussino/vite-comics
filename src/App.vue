<template>
  <HeaderComponent/>
  <main> 
  <div class="container">
    _ _> Content goes here >_ _ 
  </div>
  <BluebarComponent/>
  </main>
  <FooterComponent/>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import BluebarComponent from './components/BluebarComponent.vue';
import FooterComponent from './components/FooterComponents.vue';
export default {
  components: {
    HeaderComponent,
    FooterComponent,
    BluebarComponent
}
}
</script>

<style lang="scss" scoped>
  main {
    background-color: black;
    color: white;
    font-weight: 500;
  }

</style>