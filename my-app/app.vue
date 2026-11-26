<script setup>
// useState('key', () => {
//   return value;
// })
useState('products', () => 
  [
    {
      id: 0,
      imgUrl: '/mei-miteki.webp',
      name: '永野芽郁',
      price: 20
    },
    {
      id: 1,
      imgUrl: '/mei-1.jpg',
      name: '永野芽郁',
      price: 21
    },
    {
      id: 2,
      imgUrl: '/mei-miteki.webp',
      name: '永野芽郁',
      price: 22
    },
    {
      id: 3,
      imgUrl: '/mei-miteki.webp',
      name: '永野芽郁',
      price: 23
    },
    {
      id: 4,
      imgUrl: '/mei-miteki.webp',
      name: '永野芽郁',
      price: 1000
    }
  ]
);
</script>

<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
