<template>

  <UHeader>
    <template #title>
      <h2>E-shop</h2>
    </template>

    <UNavigationMenu :items="items" />

    <template #right>
      <UColorModeButton />

      <UTooltip text="cart" :kbds="[]">
        <UButton color="neutral" variant="ghost" to="/cart" icon="i-heroicons-shopping-cart" aria-label="السلة" />
      </UTooltip>
    </template>
  </UHeader>

</template>

<script lang="ts" setup>
import type { NavigationMenuItem } from '@nuxt/ui'

const route = useRoute()
const items = computed<NavigationMenuItem[]>(() => [
  {
    label: 'Home',
    to: '/',
    active: route.path === '/'
  },
  {
    label: 'store',
    to: '/store',
    active: route.path.startsWith('/store')
  },
  {
    label: 'categories',
    to: '/categories',

  },
  {
    label: 'Releases',
    to: 'https://github.com/nuxt/ui/releases',
    target: '_blank'
  }
])
</script>

<style></style>