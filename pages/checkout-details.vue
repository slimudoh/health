<template>
  <div class="checkout_div">
    <Header />
    <div class="checkout_div_back">
      <div>
        <nuxt-link to="checkout"> &#8592; </nuxt-link>
      </div>
      Check out
    </div>
    <div class="checkout_div_nav">
      <div
        @click="selectedInfo = 'bill'"
        :style="
          selectedInfo === 'bill'
            ? {
                borderBottom: '5px solid #F3A627',
                color: 'color: #F3A627',
                fontWeight: 'bold',
                opacity: 1,
              }
            : null
        "
      >
        Billing <br />
        Information
      </div>
      <div
        @click="selectedInfo = 'review'"
        :style="
          selectedInfo === 'review'
            ? {
                borderBottom: '5px solid #F3A627',
                color: 'color: #F3A627',
                fontWeight: 'bold',
                opacity: 1,
              }
            : null
        "
      >
        Review <br />
        & Payment
      </div>
      <div
        @click="selectedInfo = 'primary'"
        :style="
          selectedInfo === 'primary'
            ? {
                borderBottom: '5px solid #F3A627',
                color: 'color: #F3A627',
                fontWeight: 'bold',
                opacity: 1,
              }
            : null
        "
      >
        Primary <br />
        Dependent
      </div>
    </div>
    <Billing v-if="selectedInfo === 'bill'" />
    <Review v-if="selectedInfo === 'review'" />
    <Primary v-if="selectedInfo === 'primary'" />

    <div
      class="checkout_div_btn"
      @click="gotoComplete"
      v-if="selectedInfo === 'primary'"
    >
      Pay N40,000
    </div>
    <div class="checkout_div_btn" @click="gotoComplete" v-else>Continue</div>
  </div>
</template>

<script>
import Header from '@/components/HeaderEmpty'
import Billing from '@/components/Checkout/Billing'
import Review from '@/components/Checkout/Review'
import Primary from '@/components/Checkout/Primary'

export default {
  components: {
    Header,
    Billing,
    Review,
    Primary,
  },
  data() {
    return {
      selectedInfo: 'bill',
    }
  },
  methods: {
    gotoComplete() {
      this.$router.push('/complete')
    },
  },
}
</script>

<style scoped>
.checkout_div {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #ffffff;
  overflow: auto;
  padding-bottom: 100px;
}

.checkout_div_back {
  height: 70px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 30px;
  text-align: center;
  color: #f3a627;
  position: relative;
  background: #e5e5e5;
}

.checkout_div_back > div {
  position: absolute;
  top: 0;
  left: 0;
  width: 40px;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 30px;
  text-align: center;
  height: 70px;
  color: #f3a627;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.checkout_div_nav {
  background: #122933;
  padding: 0 10px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.checkout_div_nav > div {
  width: 33.33333%;
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 15px;
  text-align: center;
  color: #ffffff;
  opacity: 0.6;
  height: 60px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  border-bottom: 5px solid transparent;
}

.checkout_div_btn {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  background: #f3a627;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 24px;
  text-align: center;
  color: #ffffff;
  height: 79px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}
</style>
