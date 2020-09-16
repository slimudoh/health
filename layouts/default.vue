<template>
  <div class="container_div">
    <Header />
    <nuxt />
  </div>
</template>

<script>
import Header from '@/components/Header'

export default {
  components: {
    Header,
  },
}
</script>

<style>
@import url('~assets/css/app.css');

.container_div {
  display: none;
}

@media (max-width: 500px) {
  .container_div {
    display: block;
  }
}
</style>
