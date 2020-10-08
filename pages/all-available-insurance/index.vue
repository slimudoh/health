<template>
  <div>
    <Header />
    <div class="cover_banner">
      <div>
        <h3>Find A Health Insurance</h3>
        <p>That suits your <br />(family's) needs</p>
      </div>
    </div>
    <div class="cover_nav">
      <div>
        <div
          @click="cover = 'all'"
          :style="
            cover === 'all'
              ? {
                  fontWeight: 'bold',
                  color: '#F3A627',
                  opacity: 1,
                  borderBottom: '5px solid #f3a627',
                }
              : null
          "
        >
          All Covers
        </div>
        <div
          @click="cover = 'individual'"
          :style="
            cover === 'individual'
              ? {
                  fontWeight: 'bold',
                  color: '#F3A627',
                  opacity: 1,
                  borderBottom: '5px solid #f3a627',
                }
              : null
          "
        >
          Individual Covers
        </div>
        <div
          @click="cover = 'family'"
          :style="
            cover === 'family'
              ? {
                  fontWeight: 'bold',
                  color: '#F3A627',
                  opacity: 1,
                  borderBottom: '5px solid #f3a627',
                }
              : null
          "
        >
          Family Covers
        </div>
      </div>
    </div>

    <All v-if="cover === 'all'" />
    <Family v-if="cover === 'family'" />
    <Individual v-if="cover === 'individual'" />

    <div class="cover_connect">
      <div>
        <h3>Why HealthConnect</h3>
        <div>
          <div>
            <div>
              <svg
                width="15"
                height="16"
                viewBox="0 0 15 16"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M11.9773 1.40909H10.5682V0.704545C10.5682 0.281818 10.2864 0 9.86364 0C9.44091 0 9.15909 0.281818 9.15909 0.704545V1.40909H4.93182V0.704545C4.93182 0.281818 4.65 0 4.22727 0C3.80455 0 3.52273 0.281818 3.52273 0.704545V1.40909H2.11364C0.915909 1.40909 0 2.325 0 3.52273V13.3864C0 14.5841 0.915909 15.5 2.11364 15.5H11.9773C13.175 15.5 14.0909 14.5841 14.0909 13.3864V3.52273C14.0909 2.325 13.175 1.40909 11.9773 1.40909ZM2.1137 2.81818H3.52279V3.52272C3.52279 3.94545 3.80461 4.22727 4.22734 4.22727C4.65007 4.22727 4.93188 3.94545 4.93188 3.52272V2.81818H9.15916V3.52272C9.15916 3.94545 9.44097 4.22727 9.8637 4.22727C10.2864 4.22727 10.5682 3.94545 10.5682 3.52272V2.81818H11.9773C12.4001 2.81818 12.6819 3.1 12.6819 3.52272V5.63636H1.40916V3.52272C1.40916 3.1 1.69097 2.81818 2.1137 2.81818ZM2.1137 14.0909H11.9773C12.4001 14.0909 12.6819 13.8091 12.6819 13.3864V7.04547H1.40916V13.3864C1.40916 13.8091 1.69097 14.0909 2.1137 14.0909Z"
                  fill="black"
                />
              </svg>
            </div>
            <h3>Feature 01</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
          </div>

          <div>
            <div>
              <svg
                width="16"
                height="14"
                viewBox="0 0 16 14"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M11.1283 0C12.2748 0 13.3539 0.485149 14.1632 1.31683C15.04 2.14851 15.5121 3.32673 15.3772 4.50495C15.3772 5.68317 14.9051 6.86139 14.0958 7.69307L8.16072 13.7921C8.02584 13.9307 7.89095 14 7.68862 14C7.48628 14 7.3514 13.9307 7.21651 13.7921L1.28144 7.69307C0.472108 6.86139 0 5.68317 0 4.50495C0 3.32673 0.472108 2.14851 1.34888 1.31683C3.03498 -0.415842 5.80018 -0.415842 7.48628 1.31683L7.75606 1.59406L8.02584 1.31683C8.83516 0.485149 9.98171 0 11.1283 0ZM7.75614 12.3367L13.2191 6.72279C13.8261 6.09903 14.1633 5.33665 14.1633 4.50497C14.1633 3.67329 13.8261 2.91091 13.2866 2.28715C12.6796 1.73269 11.9377 1.38616 11.1283 1.38616C10.2516 1.38616 9.50969 1.73269 8.90269 2.28715L8.22825 3.04952C7.95847 3.32675 7.55381 3.32675 7.28403 3.04952L6.54215 2.28715C5.93515 1.66339 5.19327 1.38616 4.38394 1.38616C3.64206 1.38616 2.83273 1.66339 2.29318 2.28715C1.75363 2.91091 1.41641 3.67329 1.41641 4.50497C1.41641 5.33665 1.68618 6.09903 2.29318 6.72279L7.75614 12.3367Z"
                  fill="black"
                />
              </svg>
            </div>
            <h3>Feature 01</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
          </div>

          <div>
            <div>
              <svg
                width="11"
                height="17"
                viewBox="0 0 11 17"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M11 5.48857C11 2.46985 8.525 0 5.5 0C2.475 0 0 2.46985 0 5.48857C0 7.27235 0.825 8.85031 2.13125 9.81081L1.375 15.711C1.30625 15.9854 1.44375 16.2599 1.65 16.3971C1.85625 16.5343 2.13125 16.5343 2.40625 16.3971L5.5 14.5447L8.59375 16.3971C8.6625 16.4657 8.8 16.4657 8.9375 16.4657C9.075 16.4657 9.2125 16.3971 9.28125 16.3285C9.4875 16.1913 9.625 15.9168 9.55625 15.6424L8.8 9.81081C10.175 8.85031 11 7.27235 11 5.48857ZM1.375 5.48857C1.375 3.22454 3.23125 1.37215 5.5 1.37215C7.76875 1.37215 9.625 3.22454 9.625 5.48857C9.625 7.7526 7.76875 9.60499 5.5 9.60499C3.23125 9.60499 1.375 7.7526 1.375 5.48857ZM5.84362 13.1726L8.04362 14.4761L7.56237 10.5655C6.94362 10.8399 6.25612 10.9771 5.49987 10.9771C4.74362 10.9771 4.05612 10.8399 3.43737 10.5655L2.95612 14.4761L5.15612 13.1726C5.36237 13.0353 5.63737 13.0353 5.84362 13.1726Z"
                  fill="black"
                />
              </svg>
            </div>
            <h3>Feature 01</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
          </div>

          <div>
            <div>
              <svg
                width="16"
                height="14"
                viewBox="0 0 16 14"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M11.1283 0C12.2748 0 13.3539 0.485149 14.1632 1.31683C15.04 2.14851 15.5121 3.32673 15.3772 4.50495C15.3772 5.68317 14.9051 6.86139 14.0958 7.69307L8.16072 13.7921C8.02584 13.9307 7.89095 14 7.68862 14C7.48628 14 7.3514 13.9307 7.21651 13.7921L1.28144 7.69307C0.472108 6.86139 0 5.68317 0 4.50495C0 3.32673 0.472108 2.14851 1.34888 1.31683C3.03498 -0.415842 5.80018 -0.415842 7.48628 1.31683L7.75606 1.59406L8.02584 1.31683C8.83516 0.485149 9.98171 0 11.1283 0ZM7.75614 12.3367L13.2191 6.72279C13.8261 6.09903 14.1633 5.33665 14.1633 4.50497C14.1633 3.67329 13.8261 2.91091 13.2866 2.28715C12.6796 1.73269 11.9377 1.38616 11.1283 1.38616C10.2516 1.38616 9.50969 1.73269 8.90269 2.28715L8.22825 3.04952C7.95847 3.32675 7.55381 3.32675 7.28403 3.04952L6.54215 2.28715C5.93515 1.66339 5.19327 1.38616 4.38394 1.38616C3.64206 1.38616 2.83273 1.66339 2.29318 2.28715C1.75363 2.91091 1.41641 3.67329 1.41641 4.50497C1.41641 5.33665 1.68618 6.09903 2.29318 6.72279L7.75614 12.3367Z"
                  fill="black"
                />
              </svg>
            </div>
            <h3>Feature 01</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
          </div>
        </div>
      </div>
    </div>

    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'
import All from '@/components/Cover/AllCover'
import Family from '@/components/Cover/FamilyCover'
import Individual from '@/components/Cover/IndividualCover'

export default {
  components: {
    Footer,
    All,
    Family,
    Individual,
    Header,
  },
  data() {
    return {}
  },
  computed: {
    cover: {
      get() {
        return this.$store.state.insurance.cover
      },
      set(value) {
        this.$store.commit('insurance/UPDATE_COVER', value)
      },
    },
  },
}
</script>

<style scoped>
.cover_banner {
  background-image: url('~assets/images/banner/cover_1.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  padding: 50px 20px;
}

.cover_banner > div {
  width: 200px;
}

.cover_banner > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 26px;
  line-height: 26px;
  color: #122933;
}

.cover_banner > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 22px;
  color: #000000;
  opacity: 0.8;
  margin-top: 10px;
}

.cover_nav {
  background: #08374b;
}

.cover_nav > div {
  margin: auto;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.cover_nav > div > div {
  width: 33.33333%;
  height: 60px;
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 16px;
  color: #ffffff;
  opacity: 0.6;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  border-bottom: 5px solid transparent;
}
/*
.cover_list {
  background: #fff;
}

.cover_list > div {
  margin: auto;
}

.cover_list > div > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
  padding: 20px 0;
}

.cover_list_img {
  width: 45%;
}

.cover_list_img > div {
  width: 90%;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.cover_list_img > div > div {
  width: 50px;
  height: 50px;
  border-radius: 60px;
}

.cover_list_details {
  width: 45%;
}

.cover_list_details > h6 {
  font-style: normal;
  font-weight: bold;
  font-size: 9px;
  line-height: 17px;
  letter-spacing: -0.2px;
  color: #8a8a8a;
}

.cover_list_details > p {
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 20px;
  letter-spacing: -0.2px;
  color: #272833;
  margin: 5px 0;
}

.cover_list_details > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 17px;
  letter-spacing: -0.4px;
  color: #2a9d8f;
}

.cover_list_details > h5 {
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 16px;
  display: flex;
  align-items: center;
  text-align: left;
  text-transform: uppercase;
  color: #f3a627;
  margin-top: 10px;
}

.cover_list_details > h5 > a > span {
  text-decoration-line: underline;
  width: 100px;
} */

.cover_connect {
  background: #122933;
}

.cover_connect > div {
  width: 90%;
  margin: auto;
  padding: 30px 0;
}

.cover_connect > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 27px;
  text-align: center;
  color: #ffffff;
}

.cover_connect > div > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.cover_connect > div > div > div {
  width: 45%;
  margin-top: 20px;
}

.cover_connect > div > div > div > div {
  width: 35px;
  height: 35px;
  background: #f3a627;
  border-radius: 60px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.cover_connect > div > div > div > h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 22px;
  color: #ffffff;
  margin: 10px 0;
}

.cover_connect > div > div > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 22px;
  color: #ffffff;
}
</style>
