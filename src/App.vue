<script>
  import NavbarComponent from './components/NavbarComponent.vue';
  import ProductsComponent from './components/ProductsComponent.vue';
  import CartComponent from './components/CartComponent.vue';

  export default{
    components:{
      NavbarComponent,
      ProductsComponent,
      CartComponent
    }
  }
</script>

<template>
  <div class="container">
    <NavbarComponent></NavbarComponent>
    <CartComponent></CartComponent>
    <ProductsComponent></ProductsComponent>
  </div>
</template>

<style lang="scss">
  @import"./assets/all.scss";
  .card-img-top {
    object-fit: cover;
    height: 200px;
  }
  .table-image {
    width: 75px;
    height: 75px;
    object-fit: cover;
  }
</style>
