<template>
  <div class="website_header">
    <div>
      <div class="website_header_logo">
        <nuxt-link to="/">
          <img src="@/assets/images/logo.png" alt="logo" />
        </nuxt-link>
      </div>
      <div class="website_header_menu">
        <div @click="gotoCart">
          <div>
            <svg
              width="21"
              height="21"
              viewBox="0 0 21 21"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M3.65773 1.82583H0.874989C0.391746 1.82583 0 1.4171 0 0.912914C0 0.408725 0.391746 0 0.874989 0H4.37494C4.79199 0 5.15107 0.307091 5.23291 0.733748L5.9678 4.56457H20.1247C20.6737 4.56457 21.0871 5.08588 20.9842 5.6485L19.583 13.3147C19.3353 14.6159 18.2293 15.5448 16.9748 15.5195L8.48665 15.5194C7.21536 15.5448 6.1094 14.6159 5.86194 13.316L4.40013 5.69586C4.3942 5.67065 4.38928 5.64503 4.3854 5.61905L3.65773 1.82583ZM6.12488 19.1727C6.12488 20.2691 6.8243 21 7.87343 21C8.92256 21 9.62198 20.2691 9.62198 19.1727C9.62198 18.0763 8.92256 17.3454 7.87343 17.3454C6.8243 17.3454 6.12488 18.0763 6.12488 19.1727ZM15.75 19.1712C15.75 20.2667 16.4494 20.9971 17.4985 20.9971C18.5477 20.9971 19.2471 20.2667 19.2471 19.1712C19.2471 18.0757 18.5477 17.3454 17.4985 17.3454C16.4494 17.3454 15.75 18.0757 15.75 19.1712ZM7.57832 12.959L6.31824 6.39038H19.0673L17.8654 12.9658C17.7841 13.3927 17.4155 13.7023 16.9917 13.6939L8.47007 13.6937C8.02954 13.7023 7.66089 13.3927 7.57832 12.959Z"
                fill="#F5F4FF"
              />
            </svg>
          </div>
          <p>cart</p>
        </div>
        <div @click="mobileMenu = true">
          <div>
            <svg
              width="29"
              height="17"
              viewBox="0 0 29 17"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect width="29" height="2.68421" fill="#F5F4FF" />
              <rect y="7.15796" width="29" height="2.68421" fill="#F5F4FF" />
              <rect y="14.3157" width="29" height="2.68421" fill="#F5F4FF" />
            </svg>
          </div>
          <p>Menu</p>
        </div>
      </div>

      <div class="website_header_nav" v-if="mobileMenu">
        <div>
          <div class="website_header_nav_top">
            <div class="website_header_logo">
              <img src="@/assets/images/logo.png" alt />
            </div>
            <div class="website_header_close">
              <div @click="mobileMenu = !mobileMenu">
                <svg
                  width="17"
                  height="17"
                  viewBox="0 0 17 17"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M15.619 3.44834L10.9536 8.11375L15.619 12.7792C16.4303 13.5905 16.4303 14.8076 15.619 15.619C15.2133 16.0246 14.8076 16.2275 14.1991 16.2275C13.5905 16.2275 13.1848 16.0246 12.7792 15.619L8.11375 10.9536L3.44834 15.619C3.04265 16.0246 2.63697 16.2275 2.02844 16.2275C1.41991 16.2275 1.01422 16.0246 0.608531 15.619C-0.202844 14.8076 -0.202844 13.5905 0.608531 12.7792L5.27394 8.11375L0.608531 3.44834C-0.202844 2.63697 -0.202844 1.41991 0.608531 0.608531C1.41991 -0.202844 2.63697 -0.202844 3.44834 0.608531L8.11375 5.27394L12.7792 0.608531C13.5905 -0.202844 14.8076 -0.202844 15.619 0.608531C16.4303 1.41991 16.4303 2.63697 15.619 3.44834Z"
                    fill="white"
                  />
                </svg>
              </div>
              <p>Close</p>
            </div>
          </div>

          <div class="website_header_nav_main">
            <div @click="mobileMenu = !mobileMenu">
              <nuxt-link to="/">Home</nuxt-link>
            </div>
            <div @click="mobileMenu = !mobileMenu">
              <nuxt-link to="/all-available-insurance"
                >Find Health Insurance</nuxt-link
              >
            </div>
            <div @click="mobileMenu = !mobileMenu">
              <nuxt-link to="/all-available-clinics"
                >Find Available Clinics</nuxt-link
              >
            </div>
            <div @click="mobileMenu = !mobileMenu">
              <nuxt-link to="/about-us">About Us</nuxt-link>
            </div>
          </div>
          <div class="website_header_nav_policy">
            <div @click="mobileMenu = !mobileMenu">
              <nuxt-link to="/">FAQ</nuxt-link>
            </div>
            <div @click="mobileMenu = !mobileMenu">
              <nuxt-link to="/">Contact Us</nuxt-link>
            </div>
          </div>
          <div class="website_header_nav_copy">
            <div>© 2020 HealthConnect. All Rights Reserved.</div>
          </div>
        </div>
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
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.website_header_logo {
  width: 90px;
}

.website_header_logo > img {
  width: 100%;
}

.website_header_menu {
  width: 100px;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.website_header_menu > div {
  width: 40px;
  display: flex;
  flex-flow: column nowrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.website_header_menu > div > div {
  width: 30px;
  height: 25px;
  overflow: hidden;
  margin-bottom: 2px;
}

.website_header_menu > div > p {
  font-style: normal;
  font-weight: bold;
  font-size: 10px;
  line-height: 14px;
  text-align: center;
  text-transform: uppercase;
  color: #f5f4ff;
}

.website_header_nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #f3a627;
  z-index: 99999;
  overflow: auto;
}

.website_header_nav > div {
  width: 90%;
  margin: auto;
}

.website_header_nav_top {
  padding: 5px 0;
  margin: auto;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.website_header_close {
  width: 30px;
}

.website_header_close > div {
  width: 30px;
  height: 20px;
}

.website_header_close > p {
  font-style: normal;
  font-weight: bold;
  font-size: 10px;
  line-height: 14px;
  text-align: center;
  text-transform: uppercase;
  color: #f5f4ff;
}

.website_header_nav_main {
  margin-top: 50px;
}

.website_header_nav_main > div {
  font-style: normal;
  font-weight: normal;
  font-size: 25px;
  line-height: 34px;
  display: flex;
  align-items: center;
  color: #312828;
  margin-bottom: 20px;
}

.website_header_nav_main > div > a {
  color: #312828;
}

.website_header_nav_policy {
  margin-top: 70px;
  margin-bottom: 30px;
}

.website_header_nav_policy > div {
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 27px;
  display: flex;
  align-items: center;
  color: #312828;
  margin-bottom: 20px;
}

.website_header_nav_copy {
  position: absolute;
  bottom: 0;
  left: 0;
  padding-left: 20px;
  width: 100%;
}

@media (max-height: 480px) {
  .website_header_nav_copy {
    position: relative;
  }
}

.website_header_nav_copy > div {
  margin: auto;
  padding-bottom: 20px;
}
</style>
