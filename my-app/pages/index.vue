<script setup>
// const products = [
//   {
//     id: 0,
//     imgUrl: '/mei-miteki.webp',
//     name: '永野芽郁',
//     price: 20
//   },
//   {
//     id: 1,
//     imgUrl: '/mei-1.jpg',
//     name: '永野芽郁',
//     price: 21
//   },
//   {
//     id: 2,
//     imgUrl: '/mei-miteki.webp',
//     name: '永野芽郁',
//     price: 22
//   },
//   {
//     id: 3,
//     imgUrl: '/mei-miteki.webp',
//     name: '永野芽郁',
//     price: 23
//   },
//   {
//     id: 4,
//     imgUrl: '/mei-miteki.webp',
//     name: '永野芽郁',
//     price: 1000
//   }
// ]
const products = useState('products');

useHead({
    title: 'DTFNTR - 目黒のアンティーク家具専門店'
})
</script>

<template>
    <section class="products">
      <h2>Our Products</h2>
      <ul>
        <li v-for="product in products" :key="product.id">
          <!-- <NuxtLink to="/products/0"> -->
          <NuxtLink :to="`/products/${product.id}`">
            <img :src="product.imgUrl" alt="永野芽郁">
            <h3>{{ product.name }}</h3>
            <p>({{ product.price.toLocaleString() }})</p>
          </NuxtLink>
        </li>
      </ul>
    </section>
</template>

<style scoped>
.products h2 {
  margin-top: 32px;
}

.products ul {
  margin: 32px 0 0;
  padding: 0;
  list-style: none;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 32px;
}

.products a {
  display: block;
}

.products img {
  width: 200px;
  height: auto;
}

.products h3 {
  margin-top: 8px;
}
</style>