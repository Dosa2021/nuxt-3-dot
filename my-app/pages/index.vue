<script setup>
useHead({
    title: 'DTFNTR - 目黒のアンティーク家具専門店'
})
</script>

<template>
    <section class="products">
      <h2>Our Products</h2>
      <ul>
        <li>
          <NuxtLink to="/">
            <img src="/mei-miteki.webp" alt="永野芽郁">
            <h3>永野芽郁</h3>
            <p>25</p>
          </NuxtLink>
        </li>
        <li>
          <NuxtLink to="/">
            <img src="/mei-miteki.webp" alt="永野芽郁">
            <h3>永野芽郁</h3>
            <p>25</p>
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