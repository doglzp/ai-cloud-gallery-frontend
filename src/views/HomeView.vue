<template>
  <div class="home">
    <h1>This is an home page</h1>
  </div>
</template>

<script setup lang="ts">
import { healthUsingGet } from '@/api/mainController'

healthUsingGet().then((res) => {
  console.log(res)
})

</script>

<style>
@media (min-width: 1024px) {
  .home {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
