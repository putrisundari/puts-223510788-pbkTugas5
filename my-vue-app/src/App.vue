<template>
  <div id="app">
    <Navbar />
    <Carousel />

    <div class="product-container">
      <ProductCard
        v-for="product in products"
        :key="product.id"
        :product="product"
        @add-to-cart="handleAddToCart"
      />
    </div>

    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Carousel from './components/Carousel.vue';
import ProductCard from './components/ProductCard.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    ProductCard,
    Footer
  },
  data() {
    return {
      products: [
        { id: 1, name: 'Hoddie', price: 'Rp699.000', imgSrc: 'https://cf.shopee.co.id/file/c1d7b4c31053d1af0b6ed01db0829e85 ' },
        { id: 2, name: 'Sweater', price: 'Rp499.000', imgSrc: 'https://cf.shopee.co.id/file/52955181d73c74c1adfd7035c0f28c3e' },
        { id: 3, name: 'Blazer', price: 'Rp749.000', imgSrc: 'https://cf.shopee.co.id/file/968fb0f8ae10ff8205e83ed7dfc535aa' }
      ]
    };
  },
  methods: {
    handleAddToCart(product) {
      // Implementasikan logika untuk menambahkan produk ke keranjang
      console.log('Tambah ke keranjang:', product);
    }
  }
}
</script>

<style>
body {
  background-color: #f8f9fa;
  margin: 0;
  font-family: Arial, sans-serif;
}

.product-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 20px;
}
</style>