<template>
  <div class="website_footer_copy">
    © 2020 HealthConnect. All Rights Reserved.
  </div>
</template>

<script>
export default {
  data() {
    return {
      mobileMenu: false,
    }
  },
}
</script>

<style scoped>
.website_footer_copy {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  background: #1c2427;
  height: 57px;
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  font-style: normal;
  font-weight: normal;
  font-size: 12.4366px;
  line-height: 21px;
  color: rgba(255, 255, 255, 0.3);
}
</style>
