<script setup>
useHead({
    title: 'Index Page'
})
</script>

<template>
  <div>
    <Header />
    <p>Index Page</p>
    <NuxtLink to="/about">To About</NuxtLink>
    <Footer />
  </div>
</template>
