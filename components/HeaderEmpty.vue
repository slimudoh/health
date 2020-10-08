<template>
  <div class="website_header">
    <div>
      <div class="website_header_logo">
        <nuxt-link to="/">
          <img src="@/assets/images/logo.png" alt="logo" />
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mobileMenu: false,
    }
  },
  methods: {
    gotoCart() {
      this.$router.push('/cart')
    },
  },
}
</script>

<style scoped>
.website_header {
  background: #f3a627;
  box-shadow: inset 0px -1px 0px #f0f0f0;
}

.website_header > div {
  padding: 5px 0;
  width: 90%;
  margin: auto;
}

.website_header_logo {
  width: 90px;
  margin: auto;
}

.website_header_logo > img {
  width: 100%;
}
</style>
