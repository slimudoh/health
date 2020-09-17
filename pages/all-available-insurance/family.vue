<template>
  <div>
    <Header />
    <div class="family">
      <div class="family_banner_back">
        <nuxt-link to="/all-available-insurance">
          &#8592; Back to home
        </nuxt-link>
      </div>
      <div class="family_banner"></div>
      <div class="family_details">
        <div>
          <div>
            <div class="family_details_text">
              <div class="family_details_text_img">
                <div><img src="@/assets/images/lagos.png" alt="" /></div>
              </div>
              <div class="family_details_text_txt">
                <h6>FAMILY COVER</h6>
                <p>The Lagos State Health Scheme</p>
              </div>
            </div>
            <div class="family_details_table">
              <div class="family_details_table_top">
                <p>
                  N40,000

                  <span>per year</span>
                </p>
                <div>
                  <h6>Covers for one household of:</h6>
                  <p>
                    1 Primary Member (Above 18 years)1 Spouse and Up till 4
                    Children below 18 years
                  </p>
                </div>
              </div>
              <div class="family_details_table_btm">
                Additional Spouse(s) & Children can be added at an extra cost.
              </div>
            </div>
          </div>
        </div>
      </div>
      <Accordion />
      <div class="family_buy" @click="buyNow">Buy Now</div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'
import Accordion from '@/components/Cover/Accordion'

export default {
  components: {
    Footer,
    Accordion,
    Header,
  },
  methods: {
    buyNow() {
      this.$router.push('/checkout')
    },
  },
}
</script>

<style>
.family {
  background: #e5e5e5;
  padding-bottom: 70px;
}

.family_banner_back {
  width: 90%;
  margin: auto;
  padding: 5px 0;
  font-style: normal;
  font-weight: bold;
  font-size: 11px;
  line-height: 18px;
  color: #122933;
}

.family_banner {
  height: 178px;
  background-image: url('~assets/images/banner/family.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

.family_details > div {
  width: 90%;
  margin: auto;
  position: relative;
}

.family_details > div {
  height: 300px;
}

.family_details > div > div {
  position: absolute;
  top: -20px;
  left: 0;
  width: 100%;
  background: #fafefd;
  border: 2px solid #2a9d8f;
  box-sizing: border-box;
  padding: 20px;
}

.family_details_text {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.family_details_text_img {
  width: 90px;
}

.family_details_text_img > div {
  width: 60px;
  height: 60px;
}

.family_details_text_txt {
  width: calc(100% - 90px);
}

.family_details_text_txt > h6 {
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 16px;
  color: #2a9d8f;
}

.family_details_text_txt > p {
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 33px;
  color: #122933;
  margin-top: 10px;
}

.family_details_table_top {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  border-left: 1px solid rgba(0, 0, 0, 0.1);
  border-top: 1px solid rgba(0, 0, 0, 0.1);
  border-right: 1px solid rgba(0, 0, 0, 0.1);
  margin-top: 20px;
}

.family_details_table_top > p {
  width: 80px;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 24px;
  color: #f3a627;
}

.family_details_table_top > p > span {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 24px;
  color: #122933;
  opacity: 0.7;
}

.family_details_table_top > div {
  width: calc(100% - 100px);
  border-left: 1px solid rgba(0, 0, 0, 0.1);
  padding: 5px;
}

.family_details_table_top > div > h6 {
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 24px;
  color: #122933;
}

.family_details_table_top > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 18px;
  color: #122933;
  opacity: 0.7;
  margin-top: 5px;
}

.family_details_table_btm {
  font-style: normal;
  font-weight: normal;
  font-size: 9.5px;
  line-height: 18px;
  color: #0d0d28;
  opacity: 0.78;
  padding: 5px;
  border: 1px solid rgba(0, 0, 0, 0.1);
}

.family_buy {
  background: #f3a627;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 24px;
  color: #ffffff;
  height: 60px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}
</style>
