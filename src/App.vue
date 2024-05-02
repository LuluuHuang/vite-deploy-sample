<script>
  import NavbarComponent from './components/NavbarComponent.vue';
  import ProductsComponent from './components/ProductsComponent.vue';
  export default{
    components:{
      NavbarComponent,
      ProductsComponent
    }
  }
</script>

<template>
  <div class="container">
    <NavbarComponent></NavbarComponent>
    <ProductsComponent></ProductsComponent>
  </div>
</template>

<style lang="scss">
  @import"./assets/all.scss";
</style>
