<template>
  <div class="checkout_bill">
    <div>
      <h3>Please provide your information</h3>
      <div>
        <div>
          <label>First Name</label>
          <div>
            <input type="text" placeholder="Enter your first name" />
          </div>
        </div>

        <div>
          <label>Last Name</label>
          <div>
            <input type="text" placeholder="Enter your last name" />
          </div>
        </div>

        <div>
          <label>Your Email</label>
          <div>
            <input type="text" placeholder="Enter your last name" />
          </div>
        </div>
      </div>
      <p>We will send the order confirmation to this email address.</p>
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
  font-size: 12px;
  line-height: 18px;
  color: #000000;
  opacity: 0.4;
  text-align: center;
  margin-top: 10px;
}

.checkout_bill > div > div {
  margin-top: 30px;
}

.checkout_bill > div > div > div {
  margin-top: 20px;
}

.checkout_bill > div > div > div > label {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 24px;
  color: #000000;
}

.checkout_bill > div > div > div > div {
  background: #ffffff;
  box-sizing: border-box;
  border-radius: 2px;
  margin-top: 10px;
  border: 0;
}

.checkout_bill > div > div > div > div > input {
  height: 45px;
  background: transparent;
  border: 1.2949px solid rgba(243, 166, 39, 0.4);
  padding: 0 5px;
  outline: 1.2949px solid #f3a627;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 24px;
  color: #000000;
  opacity: 0.8;
}
</style>
