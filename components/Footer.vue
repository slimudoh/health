<template>
  <div>
    <div class="website_footer">
      <div class="website_footer_top">
        <div><img src="@/assets/images/footer.png" alt="logo" /></div>
        <p>powered by Pharmaccess Foundation</p>
      </div>
      <div class="website_footer_btm">
        <div>
          <h3>NAVIGATION</h3>
          <div>
            <div>
              <nuxt-link to="/"> Home </nuxt-link>
            </div>
            <div><nuxt-link to="/about-us"> About </nuxt-link></div>
            <div>
              <nuxt-link to="/all-available-insurance">
                Find Insurance
              </nuxt-link>
            </div>
            <div>
              <nuxt-link to="/all-available-clinics">
                Find Hospitals
              </nuxt-link>
            </div>
          </div>
        </div>
        <div>
          <h3>INFORMATION</h3>
          <div>
            <div>
              <nuxt-link to="/"> FAQ </nuxt-link>
            </div>
            <div><nuxt-link to="/">Partners</nuxt-link></div>
            <div><nuxt-link to="/">Contact us</nuxt-link></div>
          </div>
        </div>
      </div>
    </div>
    <div class="website_footer_policy">
      <div>Privacy Policy</div>
      <div>Terms of Use</div>
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
}
</script>

<style scoped>
.website_footer {
  padding: 30px 20px;
  background: #2e383d;
}

.website_footer_top {
  border-bottom: 1px solid #ccc;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.website_footer_top > div {
  width: 90px;
}

.website_footer_top > div > img {
  width: 100%;
}

.website_footer_top > p {
  width: 150px;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 16px;
  color: #fafefd;
  opacity: 0.8;
  text-align: left;
}

.website_footer_btm {
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-content: center;
  align-items: flex-start;
}

.website_footer_btm > div {
  width: 40%;
  padding-top: 30px;
}

.website_footer_btm > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 16px;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #fafefd;
  opacity: 0.5;
  margin-bottom: 10px;
}

.website_footer_btm > div > div > div {
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 21px;
  color: #fafefd;
  mix-blend-mode: normal;
  margin-top: 10px;
}

.website_footer_btm > div > div > div > a {
  color: #fafefd;
}

.website_footer_policy {
  padding: 0 20px;
  background: #1c2427;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-content: center;
  align-items: flex-start;
}

.website_footer_policy > div {
  height: 60px;
  width: 40%;
  display: flex;
  flex-flow: row nowrap;
  justify-content: flex-start;
  align-content: center;
  align-items: center;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 21px;
  color: #fafefd;
  opacity: 0.4;
}
</style>
