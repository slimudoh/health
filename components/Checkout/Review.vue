<template>
  <div class="checkout_bill">
    <div>
      <h3>Select payment option</h3>
      <div></div>
      <p>
        By placing your order you agree to the website terms and conditions and
        our privacy policy.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style scoped>
.checkout_bill > div {
  padding: 40px 0;
  width: 90%;
  margin: auto;
}

.checkout_bill > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 17px;
  line-height: 23px;
  color: #090811;
  text-align: center;
}

.checkout_bill > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 18px;
  text-align: center;
  color: #000000;
  opacity: 0.3;
}

.checkout_bill > div > div {
  width: 90%;
  background: #f5f4ff;
  border-radius: 0px 2px 2px 2px;
  padding: 20px;
  margin: 20px auto;
}
</style>
