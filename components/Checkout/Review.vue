<template>
  <div class="checkout_bill">
    <div>
      <h3>Please enter your credit card infomation</h3>
      <!-- <div>
        <div>
          <p>
            <input type="radio" checked="checked" name="payment" />
            <span class="checkmark"></span>
          </p>
          <div>
            <h6>Pay via CreditCard</h6>
            <p>
              <img src="@/assets/images/visa.png" style="width: 150px" alt="" />
            </p>
          </div>
        </div>
        <div>
          <p>
            <input type="radio" name="payment" />
            <span class="checkmark"></span>
          </p>
          <div>
            <h6>Pay via PayPal</h6>
            <p>
              <img
                src="@/assets/images/paypal.png"
                style="width: 177px"
                alt=""
              />
            </p>
          </div>
        </div>
      </div> -->

      <div class="checkout_bill_form">
        <div class="checkout_bill_form_long">
          <label>CARD NUMBER</label>
          <input type="text" placeholder="5376 4374 4829 4092" />
          <div>
            <img src="@/assets/images/debit.svg" alt="" />
          </div>
        </div>
        <div class="checkout_bill_form_short">
          <div class="checkout_bill_form_short_month">
            <label>VALID TILL</label>
            <input type="text" placeholder="MM/YY" />
          </div>
          <div class="checkout_bill_form_short_cvv">
            <label>CVV</label>
            <input type="text" placeholder="531" />
          </div>
        </div>
      </div>
      <div class="checkout_bill_notice">
        <div>
          <svg
            width="11"
            height="13"
            viewBox="0 0 11 13"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M9.35 4.95H8.8V3.3C8.8 1.485 7.315 0 5.5 0C3.685 0 2.2 1.485 2.2 3.3V4.95H1.65C0.715 4.95 0 5.665 0 6.6V10.45C0 11.385 0.715 12.1 1.65 12.1H9.35C10.285 12.1 11 11.385 11 10.45V6.6C11 5.665 10.285 4.95 9.35 4.95ZM3.3 3.3C3.3 2.09 4.29 1.1 5.5 1.1C6.71 1.1 7.7 2.09 7.7 3.3V4.95H3.3V3.3ZM9.35 11C9.68 11 9.9 10.78 9.9 10.45V6.6C9.9 6.27 9.68 6.05 9.35 6.05H1.65C1.32 6.05 1.1 6.27 1.1 6.6V10.45C1.1 10.78 1.32 11 1.65 11H9.35Z"
              fill="white"
            />
          </svg>
        </div>
        <p>
          By placing your order you agree to the website terms and conditions
          and our privacy policy.
        </p>
      </div>
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
  max-width: 200px;
  margin: auto;
  font-style: normal;
  font-weight: bold;
  font-size: 17px;
  line-height: 23px;
  color: #090811;
  text-align: center;
}

.checkout_bill_notice {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.checkout_bill_notice > div {
  width: 34px;
  height: 34px;
  border-radius: 60px;
  background: #f3a627;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.checkout_bill_notice > p {
  width: calc(100% - 50px);
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 18px;
  /* or 129% */

  color: #000000;

  opacity: 0.3;
}

.checkout_bill_form {
  padding: 20px 0;
}

.checkout_bill_form_long {
  padding: 20px;
  background: #ffffff;
  border: 1px solid rgba(41, 41, 41, 0.3);
  box-sizing: border-box;
  border-radius: 2px;
  position: relative;
}

.checkout_bill_form_long > label {
  font-style: normal;
  font-weight: normal;
  font-size: 10px;
  line-height: 12px;
  /* identical to box height, or 120% */

  color: #464646;

  opacity: 0.4;
}

.checkout_bill_form_long > input {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 12px;
  color: #000000;
  border: 0;
  outline: 0;
  height: 20px;
  padding-top: 10px;
}

.checkout_bill_form_long > div {
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.checkout_bill_form_short {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  margin-top: 40px;
}

.checkout_bill_form_short_month {
  width: 50%;
  background: #ffffff;
  border: 1px solid rgba(41, 41, 41, 0.3);
  box-sizing: border-box;
  border-radius: 2px;
  padding: 20px;
}

.checkout_bill_form_short_month > label {
  font-style: normal;
  font-weight: normal;
  font-size: 10px;
  line-height: 12px;
  /* identical to box height, or 120% */

  color: #464646;

  opacity: 0.4;
}

.checkout_bill_form_short_month > input {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 12px;
  color: #000000;
  border: 0;
  outline: 0;
  height: 20px;
  padding-top: 10px;
}

.checkout_bill_form_short_cvv {
  width: 40%;
  background: #ffffff;
  border: 1px solid rgba(41, 41, 41, 0.3);
  box-sizing: border-box;
  border-radius: 2px;
  padding: 20px;
}

.checkout_bill_form_short_cvv > label {
  font-style: normal;
  font-weight: normal;
  font-size: 10px;
  line-height: 12px;
  /* identical to box height, or 120% */

  color: #464646;

  opacity: 0.4;
}

.checkout_bill_form_short_cvv > input {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 12px;
  color: #000000;
  border: 0;
  outline: 0;
  height: 20px;
  padding-top: 10px;
}
</style>
