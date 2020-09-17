<template>
  <div class="checkout_div">
    <Header />
    <div class="checkout_div_details">
      <div class="checkout_div_details_item">
        <div class="checkout_div_details_item_top">
          <div>
            <h3>The Lagos State Health Scheme</h3>
            <p>N40,000</p>
          </div>
          <p>
            <svg
              width="16"
              height="18"
              viewBox="0 0 16 18"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M15.2 3.2H12V2.4C12 1.04 10.96 0 9.6 0H6.4C5.04 0 4 1.04 4 2.4V3.2H0.8C0.32 3.2 0 3.52 0 4C0 4.48 0.32 4.8 0.8 4.8H1.6V15.2C1.6 16.56 2.64 17.6 4 17.6H12C13.36 17.6 14.4 16.56 14.4 15.2V4.8H15.2C15.68 4.8 16 4.48 16 4C16 3.52 15.68 3.2 15.2 3.2ZM5.6 2.4C5.6 1.92 5.92 1.6 6.4 1.6H9.6C10.08 1.6 10.4 1.92 10.4 2.4V3.2H5.6V2.4ZM12 16C12.48 16 12.8 15.68 12.8 15.2V4.8H3.2V15.2C3.2 15.68 3.52 16 4 16H12Z"
                fill="#2A9D8F"
              />
            </svg>
          </p>
        </div>
        <div class="checkout_div_details_item_btm">
          <div class="checkout_div_details_item_btm_type">
            <h6>Type:</h6>
            <p>Family Cover</p>
          </div>
          <div class="checkout_div_details_item_btm_duration">
            <h6>DURATION of cover</h6>
            <p>12 Months</p>
          </div>
        </div>
      </div>
      <div class="checkout_div_details_list">
        <div class="checkout_div_details_list_member">
          <div>
            <h6>Primary Member</h6>
            <p>1</p>
          </div>
          <p>Must reside in Nigeria & able to fill online forms</p>
        </div>
        <div class="checkout_div_details_list_spouse">
          <div>
            <p>Spouse(s)</p>
            <div>
              <div>-</div>
              <p>2</p>
              <div>+</div>
            </div>
          </div>
          <p>
            Adding more than <span>1 spouse</span> will cost an additional
            <span>N8,500</span>.
          </p>
        </div>
        <div class="checkout_div_details_list_child">
          <div>
            <p>Children</p>
            <div>
              <div>-</div>
              <p>2</p>
              <div>+</div>
            </div>
          </div>
          <p>
            Adding more than <span>4 children</span> will cost an additional
            <span>N6,000</span>.
          </p>
        </div>
      </div>
      <div class="checkout_div_details_amount">
        <div class="checkout_div_details_amount_list">
          <h6>Subtotal</h6>
          <p>N40,000</p>
        </div>
        <div class="checkout_div_details_amount_list">
          <h6>2 Additional Spouses</h6>
          <p>N8,500</p>
        </div>
        <div class="checkout_div_details_amount_list">
          <h6>Service Charge</h6>
          <p>N2,000</p>
        </div>
        <div class="checkout_div_details_amount_total">
          <h6>Total</h6>
          <p>N50,500</p>
        </div>
      </div>
    </div>
    <div class="checkout_div_details_btn">
      <div @click="viewCheckInfo">Buy Now</div>
      <p @click="viewCovers">Cancel</p>
    </div>
  </div>
</template>

<script>
import Header from '@/components/HeaderEmpty'

export default {
  components: {
    Header,
  },
  data() {
    return {}
  },
  methods: {
    viewCovers() {
      this.$router.push('/all-available-insurance')
    },
    viewCheckInfo() {
      this.$router.push('/checkout-details')
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
  background: #e5e5e5;
  overflow: auto;
  padding-bottom: 100px;
}

.checkout_div_details {
  width: 90%;
  padding-top: 20px;
  margin: auto;
  background: #e5e5e5;
}

.checkout_div_details_item {
  background: #fafefd;
  padding: 20px;
}

.checkout_div_details_item_top {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  padding-bottom: 10px;
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
}

.checkout_div_details_item_top > div {
  width: calc(100% - 30px);
}

.checkout_div_details_item_top > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 27px;
  color: #122933;
}

.checkout_div_details_item_top > div > p {
  font-style: normal;
  font-weight: bold;
  font-size: 19px;
  line-height: 24px;
  color: #f3a627;
  margin-top: 5px;
}

.checkout_div_details_item_top > p {
  width: 20px;
  text-align: right;
}

.checkout_div_details_item_btm {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  padding-top: 10px;
}

.checkout_div_details_item_btm_type {
  width: 50%;
}

.checkout_div_details_item_btm_type > h6 {
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 18px;
  text-transform: uppercase;
  color: #000000;
  opacity: 0.3;
  margin-bottom: 5px;
}

.checkout_div_details_item_btm_type > p {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 18px;
  color: #000000;
}

.checkout_div_details_item_btm_duration {
  width: 50%;
}

.checkout_div_details_item_btm_duration > h6 {
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 18px;
  text-transform: uppercase;
  color: #000000;
  opacity: 0.3;
  margin-bottom: 5px;
  text-align: right;
}

.checkout_div_details_item_btm_duration > p {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 18px;
  color: #000000;
  text-align: right;
}

.checkout_div_details_amount {
  background: #fafefd;
  margin-top: 20px;
  padding: 20px;
}

.checkout_div_details_amount_list {
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.checkout_div_details_amount_list > h6 {
  width: calc(100% - 110px);
  height: 50px;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 24px;
  color: rgba(0, 0, 0, 0.6);
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-start;
  align-content: center;
  align-items: center;
}

.checkout_div_details_amount_list > p {
  width: 100px;
  height: 50px;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 24px;
  text-align: right;
  color: #000000;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-end;
  align-content: center;
  align-items: center;
}

.checkout_div_details_amount_total {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.checkout_div_details_amount_total > h6 {
  width: 100px;
  height: 50px;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 24px;
  color: #000000;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-start;
  align-content: center;
  align-items: center;
}

.checkout_div_details_amount_total > p {
  width: calc(100% - 110px);
  height: 50px;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 24px;
  color: #000000;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-end;
  align-content: center;
  align-items: center;
}

.checkout_div_details_btn > div {
  background: #f3a627;
  height: 56px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 24px;
  color: #ffffff;
}

.checkout_div_details_btn > p {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 10px;
  text-align: center;
  text-transform: uppercase;
  color: #f3a627;
  margin-top: 30px;
}

.checkout_div_details_list {
  margin-top: 20px;
  background: #fafefd;
  padding: 20px;
}

.checkout_div_details_list_member {
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
  padding: 10px 0;
}

.checkout_div_details_list_member > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  min-height: 30px;
}

.checkout_div_details_list_member > div > p {
  width: 100px;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  line-height: 18px;
  color: #000000;
  opacity: 0.8;
  text-align: center;
}

.checkout_div_details_list_member > div > h6 {
  width: calc(100% - 100px);
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 18px;
  color: #000000;
  opacity: 0.9;
}

.checkout_div_details_list_member > p {
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 18px;
  color: #08374b;
  text-align: left;
}

.checkout_div_details_list_spouse {
  padding: 10px 0;
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
}

.checkout_div_details_list_spouse > p {
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 18px;
  color: #e49a1e;
}

.checkout_div_details_list_spouse > p > span {
  font-weight: 600;
}

.checkout_div_details_list_spouse > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  min-height: 40px;
}

.checkout_div_details_list_spouse > div > p {
  width: calc(100% - 130px);
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 18px;
  color: #000000;
  opacity: 0.89;
}

.checkout_div_details_list_spouse > div > div {
  width: 120px;
  padding: 0 5px;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.checkout_div_details_list_spouse > div > div > p {
  width: 30px;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 18px;
  color: #000000;
  opacity: 0.8;
  text-align: center;
}

.checkout_div_details_list_spouse > div > div > div {
  width: 30px;
  height: 30px;
  border-radius: 60px;
  background: #f3a627;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 18px;
  color: #ffffff;
}

.checkout_div_details_list_child {
  padding: 10px 0;
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
}

.checkout_div_details_list_child > p {
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 18px;
  color: #08374b;
}

.checkout_div_details_list_child > p > span {
  font-weight: 600;
}

.checkout_div_details_list_child > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  min-height: 40px;
}

.checkout_div_details_list_child > div > p {
  width: calc(100% - 130px);
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 18px;
  color: #000000;
  opacity: 0.89;
}

.checkout_div_details_list_child > div > div {
  width: 120px;
  padding: 0 5px;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.checkout_div_details_list_child > div > div > p {
  width: 30px;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 18px;
  color: #000000;
  opacity: 0.8;
  text-align: center;
}

.checkout_div_details_list_child > div > div > div {
  width: 30px;
  height: 30px;
  border-radius: 60px;
  background: #f3a627;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 18px;
  /* identical to box height, or 120% */

  color: #ffffff;
}
</style>
