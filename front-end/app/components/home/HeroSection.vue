<template>
  <UPageHero
    title="Eshop "
    description="Born from the struggle of finding good deals without the hassle, Eshop became the place where quality meets comfort. We started with a simple idea: make shopping easy, trustworthy, and enjoyable. Today, every product you see is carefully selected to give you the best value with zero stress. Welcome to Eshop — where the right deal always finds you."
    headline="Smash it"
    :links="links"
  />
</template>

<script lang="ts" setup>
  const links = ref([
    {
      label : 'Get Started',
      to:'/store',
      icon : 'i-lucide-square-play'
    }
  ])    
</script>

<style>

</style>