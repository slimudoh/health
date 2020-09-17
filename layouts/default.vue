<template>
  <div class="container_div">
    <nuxt />
  </div>
</template>

<script>
export default {
  components: {},
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
