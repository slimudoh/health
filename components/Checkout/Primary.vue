<template>
  <div class="checkout_bill">
    <div>
      <h3>Details of primary member</h3>
      <h6>Must reside in Nigeria & able to fill online forms</h6>
      <div>
        <div class="checkout_bill_input">
          <label>First Name</label>
          <div>
            <input type="text" placeholder="Enter your first name" />
          </div>
        </div>

        <div class="checkout_bill_input">
          <label>Last Name</label>
          <div>
            <input type="text" placeholder="Enter your last name" />
          </div>
        </div>

        <div class="checkout_bill_date">
          <label>Date of birth</label>
          <div>
            <div>
              <input type="text" placeholder="Day" />
            </div>
            <div>
              <select>
                <option>Month</option>
              </select>
              <div>
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g opacity="0.5">
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M4.99977 10.0344C5.00392 10.0949 5.00342 10.1103 5.01372 10.1702C5.03697 10.3049 5.08802 10.4344 5.16303 10.5487C5.20093 10.6065 5.24503 10.657 5.29208 10.7074L11.2923 16.7076C11.3367 16.749 11.3468 16.7606 11.3952 16.7973C11.4496 16.8386 11.5083 16.8743 11.57 16.9036C11.8396 17.0318 12.1594 17.0318 12.429 16.9036C12.4907 16.8743 12.5493 16.8386 12.6037 16.7973C12.6521 16.7606 12.6623 16.749 12.7066 16.7076L18.7069 10.7074C18.7483 10.663 18.7599 10.6529 18.7966 10.6045C18.893 10.4774 18.9581 10.3274 18.9853 10.1702C19.0046 10.0579 19.0046 9.94255 18.9853 9.8303C18.9698 9.74054 18.942 9.65299 18.9029 9.57074C18.7543 9.25832 18.4461 9.04081 18.102 9.00541C17.966 8.99146 17.8275 9.00571 17.6972 9.04707C17.5887 9.08152 17.4862 9.13457 17.3955 9.20337C17.3471 9.24012 17.3369 9.25167 17.2926 9.29308L11.9995 14.5862L6.70634 9.29308L6.65644 9.24647C6.60944 9.20822 6.59849 9.19732 6.54769 9.16402C6.45248 9.10157 6.34663 9.05557 6.23602 9.02861C6.14752 9.00706 6.05612 8.99766 5.96511 9.00076C5.61935 9.01256 5.29708 9.20857 5.12753 9.51009C5.07172 9.60934 5.03307 9.71809 5.01372 9.8303C5.00342 9.8902 5.00392 9.9056 4.99977 9.9661C4.99977 9.98886 4.99977 10.0116 4.99977 10.0344Z"
                      fill="black"
                    />
                  </g>
                </svg>
              </div>
            </div>
            <div>
              <input type="text" placeholder="Year" />
            </div>
          </div>
        </div>

        <div class="checkout_bill_input">
          <label>Phone Number</label>
          <div>
            <div>
              <div>+234</div>
            </div>
            <input type="text" style="padding-left: 50px" />
          </div>
        </div>

        <div class="checkout_bill_input">
          <label>Please Confirm Phone Number</label>
          <div>
            <div><div>+234</div></div>
            <input type="text" style="padding-left: 50px" />
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

.checkout_bill > div > h6 {
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  color: #08374b;
  opacity: 0.6;
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

.checkout_bill_input {
  margin-top: 20px;
}

.checkout_bill_input > label {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 24px;
  color: #000000;
}

.checkout_bill_input > div {
  background: #ffffff;
  box-sizing: border-box;
  border-radius: 2px;
  margin-top: 10px;
  border: 0;
  position: relative;
}

.checkout_bill_input > div > input {
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

.checkout_bill_input > div > div {
  position: absolute;
  top: 0;
  left: 0;
  width: 45px;
  height: 45px;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 24px;
  color: #000000;
  opacity: 0.8;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.checkout_bill_input > div > div > div {
  border-right: 1px solid rgba(0, 0, 0, 0.2);
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.checkout_bill_date {
  margin-top: 20px;
}

.checkout_bill_date > label {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 24px;
  color: #000000;
}

.checkout_bill_date > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  margin-top: 10px;
}

.checkout_bill_date > div > div {
  width: 30%;
  position: relative;
}

.checkout_bill_date > div > div > div {
  position: absolute;
  top: 0;
  right: 0;
  width: 45px;
  height: 45px;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 24px;
  color: #000000;
  opacity: 0.8;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.checkout_bill_date > div > div > input {
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

.checkout_bill_date > div > div > select {
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
