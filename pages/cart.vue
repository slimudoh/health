<template>
  <div>
    <Header />
    <div class="cart_div">
      <div>
        <svg
          width="70"
          height="70"
          viewBox="0 0 70 70"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle opacity="0.1" cx="35" cy="35" r="35" fill="#F3A627" />
          <path
            d="M41.3333 32.3334C41.3333 33.7479 40.7714 35.1045 39.7712 36.1047C38.771 37.1048 37.4145 37.6667 36 37.6667C34.5855 37.6667 33.229 37.1048 32.2288 36.1047C31.2286 35.1045 30.6667 33.7479 30.6667 32.3334M28 21.6667L24 27.0001V45.6667C24 47.1334 25.2 48.3334 26.6667 48.3334H45.3333C46.0406 48.3334 46.7189 48.0525 47.219 47.5524C47.719 47.0523 48 46.374 48 45.6667V27.0001L44 21.6667H28ZM25.0667 27.0001H46.9333H25.0667Z"
            stroke="#F3A627"
            stroke-width="3"
            stroke-linecap="round"
          />
        </svg>
      </div>
      <p>No order at the moment</p>
      <button @click="viewCovers">View Covers</button>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Right'

export default {
  components: {
    Header,
    Footer,
  },
  data() {
    return {}
  },
  methods: {
    viewCovers() {
      this.$router.push('/all-available-insurance')
    },
  },
}
</script>

<style scoped>
.cart_div {
  width: 90%;
  height: 400px;
  margin: auto;
}

.cart_div > div {
  width: 70px;
  height: 70px;
  border-radius: 60px;
  margin: auto;
  margin-top: 150px;
}

.cart_div > p {
  width: 200px;
  margin: auto;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 30px;
  text-align: center;
  color: #122933;
  margin-top: 30px;
}

.cart_div > button {
  background: #f3a627;
  border-radius: 5px;
  height: 58px;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 24px;
  text-align: center;
  color: #ffffff;
  margin-top: 50px;
}
</style>
