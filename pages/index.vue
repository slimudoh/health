<template>
  <div>
    <Header />
    <div class="home_banner">
      <div>
        <img src="@/assets/images/banner/home.png" alt="" />

        <div class="home_banner_text">
          <h3>
            Keep your family <br />
            back home healthy!
          </h3>
          <p>
            Protect them from health emergencies, <br />
            and give yourself peace of mind.
          </p>
          <div>
            <nuxt-link to="/all-available-insurance">
              <div>FIND A health INSURAnce</div>
            </nuxt-link>
          </div>
        </div>

        <div class="home_banner_img_one">
          <img src="@/assets/images/home/img_1.png" alt="" />
        </div>
        <div class="home_banner_img_two">
          <img src="@/assets/images/home/img_2.png" alt="" />
        </div>
        <div class="home_banner_img_three">
          <img src="@/assets/images/home/img_3.png" alt="" />
        </div>
        <div class="home_banner_img_four">
          <img src="@/assets/images/home/img_4.png" alt="" />
        </div>
        <div class="home_banner_img_five">
          <img src="@/assets/images/home/img_5.png" alt="" />
        </div>
      </div>
    </div>
    <div class="home_insurance">
      <div class="home_insurance_list">
        <h3>Available Health Insurances</h3>
        <div>
          <div @click="gotoFam">
            <div>
              <div><img src="@/assets/images/family.png" alt="" /></div>
              <div><img src="@/assets/images/lagos.png" alt="" /></div>
            </div>
            <h6>FAMILY COVER</h6>
            <p>The Lagos State Health Scheme</p>
            <h3>N40,000</h3>
          </div>
          <div @click="gotoInd">
            <div>
              <div><img src="@/assets/images/lady.png" alt="" /></div>
              <div><img src="@/assets/images/lagos.png" alt="" /></div>
            </div>
            <h6>INDIVIDUAL COVER</h6>
            <p>The Lagos State Health Scheme</p>
            <h3>N8,500</h3>
          </div>
        </div>
      </div>
      <div class="home_insurance_partner">
        <h3>Our Partners</h3>
        <div>
          <client-only>
            <carousel :autoplay="true" :nav="false" :dots="false">
              <div class="home_insurance_partner_img">
                <div style="padding: 0 20px">
                  <img src="@/assets/images/slider/img_1.png" alt="" />
                </div>
              </div>
              <div class="home_insurance_partner_img">
                <div>
                  <img src="@/assets/images/slider/img_2.png" alt="" />
                </div>
              </div>
              <div class="home_insurance_partner_img">
                <div>
                  <img src="@/assets/images/slider/img_3.png" alt="" />
                </div>
              </div>
              <div class="home_insurance_partner_img">
                <div>
                  <img src="@/assets/images/slider/img_4.png" alt="" />
                </div>
              </div>
            </carousel>
          </client-only>
        </div>
      </div>
    </div>
    <div class="home_connect">
      <h3>Why HealthConnect</h3>
      <div>
        <div>
          <p>
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
          </p>
          <div>
            <h6>Feature 01</h6>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
          </div>
        </div>
        <div>
          <p>
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
          </p>
          <div>
            <h6>Feature 02</h6>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
          </div>
        </div>
        <div>
          <p>
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
          </p>
          <div>
            <h6>Feature 03</h6>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
          </div>
        </div>
      </div>
    </div>
    <div class="home_clinic">
      <div>
        <div>
          <img src="@/assets/images/clinic.svg" alt="" />
          <h3>Find Available Clinics</h3>
          <p>
            Find out which private and public clinics your relatives can access
            if you gift them a health insurance.
          </p>
          <div>
            <nuxt-link to="/all-available-clinics">
              <div>
                <svg
                  width="13"
                  height="15"
                  viewBox="0 0 13 15"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M6.335 14.3333C6.335 14.3333 1.00167 11.3333 1.00167 6.46667C0.983873 5.75514 1.10868 5.04726 1.36872 4.38472C1.62877 3.72218 2.0188 3.11839 2.51583 2.60894C3.01286 2.09948 3.60683 1.69467 4.26275 1.41834C4.91866 1.14202 5.62326 0.999778 6.335 1C7.04675 0.999778 7.75134 1.14202 8.40725 1.41834C9.06317 1.69467 9.65714 2.09948 10.1542 2.60894C10.6512 3.11839 11.0412 3.72218 11.3013 4.38472C11.5613 5.04726 11.6861 5.75514 11.6683 6.46667C11.6683 11.3333 6.335 14.3333 6.335 14.3333Z"
                    stroke="black"
                    stroke-linecap="round"
                  />
                  <path
                    d="M6.33496 8.33325C7.43953 8.33325 8.33496 7.43782 8.33496 6.33325C8.33496 5.22868 7.43953 4.33325 6.33496 4.33325C5.23039 4.33325 4.33496 5.22868 4.33496 6.33325C4.33496 7.43782 5.23039 8.33325 6.33496 8.33325Z"
                    stroke="black"
                    stroke-linecap="round"
                  />
                </svg>
                Find available clinics
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div class="home_power">
      <div>
        <h3>Empowering you to look after your loved ones</h3>
        <p>
          In just a few simple steps, HealthConnect allows you to directly
          activate a health cover for your family back home, by digitally
          connecting to African health insurance schemes.
        </p>
        <div>
          <nuxt-link to="/about-us">
            <div>ABOUT HEALTHCONNECT</div>
          </nuxt-link>
        </div>
      </div>
    </div>
    <div class="home_video">
      <div>
        <div>
          <svg
            width="9"
            height="12"
            viewBox="0 0 9 12"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path d="M9 6L0 11.1962L0 0.803848L9 6Z" fill="#FAFEFD" />
          </svg>
        </div>
      </div>
      <p>
        “It’s relieving to discover that I can directly take control over the
        healthcare needs of my aged mother, all-year round”.
      </p>
      <h5>Seun Olamiji</h5>
      <h6>London</h6>
    </div>
    <div class="home_rate">
      <h3>See What Others Are Saying</h3>
      <div>
        <div>
          <div class="home_rate_list">
            <svg
              width="10"
              height="10"
              viewBox="0 0 10 10"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M5.196 0.128211L6.62287 3.16057L9.81252 3.64695C9.89509 3.65979 9.96358 3.72041 9.9893 3.80344C10.015 3.88646 9.99353 3.97755 9.93383 4.03855L7.62622 6.3984L8.17106 9.73122C8.18538 9.81717 8.15172 9.90416 8.08426 9.95551C8.0168 10.0069 7.92727 10.0137 7.85342 9.97305L5.00033 8.39982L2.14723 9.9735C2.07343 10.0143 1.98385 10.0076 1.91635 9.95624C1.84885 9.9049 1.81519 9.81786 1.82959 9.7319L2.37443 6.3984L0.0661682 4.03855C0.00646863 3.97755 -0.0150217 3.88646 0.0106988 3.80344C0.0364193 3.72041 0.104911 3.65979 0.187484 3.64695L3.37713 3.16057L4.80466 0.128211C4.84098 0.0498014 4.91699 0 5.00033 0C5.08366 0 5.15967 0.0498014 5.196 0.128211Z"
                fill="#FA8231"
              />
            </svg>
            <svg
              width="10"
              height="10"
              viewBox="0 0 10 10"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M5.196 0.128211L6.62287 3.16057L9.81252 3.64695C9.89509 3.65979 9.96358 3.72041 9.9893 3.80344C10.015 3.88646 9.99353 3.97755 9.93383 4.03855L7.62622 6.3984L8.17106 9.73122C8.18538 9.81717 8.15172 9.90416 8.08426 9.95551C8.0168 10.0069 7.92727 10.0137 7.85342 9.97305L5.00033 8.39982L2.14723 9.9735C2.07343 10.0143 1.98385 10.0076 1.91635 9.95624C1.84885 9.9049 1.81519 9.81786 1.82959 9.7319L2.37443 6.3984L0.0661682 4.03855C0.00646863 3.97755 -0.0150217 3.88646 0.0106988 3.80344C0.0364193 3.72041 0.104911 3.65979 0.187484 3.64695L3.37713 3.16057L4.80466 0.128211C4.84098 0.0498014 4.91699 0 5.00033 0C5.08366 0 5.15967 0.0498014 5.196 0.128211Z"
                fill="#FA8231"
              />
            </svg>
            <svg
              width="10"
              height="10"
              viewBox="0 0 10 10"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M5.196 0.128211L6.62287 3.16057L9.81252 3.64695C9.89509 3.65979 9.96358 3.72041 9.9893 3.80344C10.015 3.88646 9.99353 3.97755 9.93383 4.03855L7.62622 6.3984L8.17106 9.73122C8.18538 9.81717 8.15172 9.90416 8.08426 9.95551C8.0168 10.0069 7.92727 10.0137 7.85342 9.97305L5.00033 8.39982L2.14723 9.9735C2.07343 10.0143 1.98385 10.0076 1.91635 9.95624C1.84885 9.9049 1.81519 9.81786 1.82959 9.7319L2.37443 6.3984L0.0661682 4.03855C0.00646863 3.97755 -0.0150217 3.88646 0.0106988 3.80344C0.0364193 3.72041 0.104911 3.65979 0.187484 3.64695L3.37713 3.16057L4.80466 0.128211C4.84098 0.0498014 4.91699 0 5.00033 0C5.08366 0 5.15967 0.0498014 5.196 0.128211Z"
                fill="#FA8231"
              />
            </svg>
            <svg
              width="10"
              height="10"
              viewBox="0 0 10 10"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M5.196 0.128211L6.62287 3.16057L9.81252 3.64695C9.89509 3.65979 9.96358 3.72041 9.9893 3.80344C10.015 3.88646 9.99353 3.97755 9.93383 4.03855L7.62622 6.3984L8.17106 9.73122C8.18538 9.81717 8.15172 9.90416 8.08426 9.95551C8.0168 10.0069 7.92727 10.0137 7.85342 9.97305L5.00033 8.39982L2.14723 9.9735C2.07343 10.0143 1.98385 10.0076 1.91635 9.95624C1.84885 9.9049 1.81519 9.81786 1.82959 9.7319L2.37443 6.3984L0.0661682 4.03855C0.00646863 3.97755 -0.0150217 3.88646 0.0106988 3.80344C0.0364193 3.72041 0.104911 3.65979 0.187484 3.64695L3.37713 3.16057L4.80466 0.128211C4.84098 0.0498014 4.91699 0 5.00033 0C5.08366 0 5.15967 0.0498014 5.196 0.128211Z"
                fill="#FA8231"
              />
            </svg>
            <svg
              width="10"
              height="10"
              viewBox="0 0 10 10"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M5.196 0.128211L6.62287 3.16057L9.81252 3.64695C9.89509 3.65979 9.96358 3.72041 9.9893 3.80344C10.015 3.88646 9.99353 3.97755 9.93383 4.03855L7.62622 6.3984L8.17106 9.73122C8.18538 9.81717 8.15172 9.90416 8.08426 9.95551C8.0168 10.0069 7.92727 10.0137 7.85342 9.97305L5.00033 8.39982L2.14723 9.9735C2.07343 10.0143 1.98385 10.0076 1.91635 9.95624C1.84885 9.9049 1.81519 9.81786 1.82959 9.7319L2.37443 6.3984L0.0661682 4.03855C0.00646863 3.97755 -0.0150217 3.88646 0.0106988 3.80344C0.0364193 3.72041 0.104911 3.65979 0.187484 3.64695L3.37713 3.16057L4.80466 0.128211C4.84098 0.0498014 4.91699 0 5.00033 0C5.08366 0 5.15967 0.0498014 5.196 0.128211Z"
                fill="#FA8231"
              />
            </svg>
          </div>
          <div class="home_rate_para">
            “It’s relieving to discover that I can directly take control over
            the healthcare needs of my aged mother, all-year round”.
          </div>
          <div class="home_rate_details">
            <p>
              <img src="@/assets/images/oval.png" alt="" />
            </p>
            <div>
              <h3>Adeola James</h3>
              <p>From London</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Newsletter />
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'
import Newsletter from '@/components/Newsletter'

export default {
  components: {
    Footer,
    Header,
    Newsletter,
    carousel:
      typeof window !== 'undefined' ? () => import('vue-owl-carousel') : '',
  },
  methods: {
    gotoFam() {
      this.cover = 'family'
      this.$router.push('/all-available-insurance')
    },
    gotoInd() {
      this.cover = 'individual'
      this.$router.push('/all-available-insurance')
    },
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
.home_banner > div {
  position: relative;
}

.home_banner_text {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: transparent;
  padding-top: 100px;
  z-index: 5;
}

.home_banner_text > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 25px;
  line-height: 28px;
  text-align: center;
  color: #08374b;
  width: 250px;
  margin: 20px auto;
}

.home_banner_text > p {
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 23px;
  text-align: center;
  color: #08374b;
  width: 90%;
  margin: 20px auto;
}

.home_banner_text > div {
  background: #f3a627;
  border-radius: 5px;
  width: 200px;
  margin: auto;
}

.home_banner_text > div > a > div {
  height: 55px;
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 16px;
  text-transform: uppercase;
  color: #122933;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.home_banner_img_one {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: transparent;
  text-align: center;
}

.home_banner_img_one > img {
  width: 70px;
}

.home_banner_img_two {
  position: absolute;
  top: 50px;
  left: 0;
  width: 70px;
  background: transparent;
  text-align: left;
}

.home_banner_img_two > img {
  width: 60px;
}

.home_banner_img_three {
  position: absolute;
  top: 50px;
  right: 0;
  width: 70px;
  background: transparent;
  text-align: right;
}

.home_banner_img_three > img {
  width: 60px;
}

.home_banner_img_four {
  position: absolute;
  bottom: 20px;
  left: 0;
  width: 70px;
  background: transparent;
  text-align: left;
}

.home_banner_img_four > img {
  width: 60px;
}

.home_banner_img_five {
  position: absolute;
  bottom: 50px;
  right: 0;
  width: 70px;
  background: transparent;
  text-align: right;
}

.home_banner_img_five > img {
  width: 60px;
}

.home_insurance {
  background: #fff;
  padding: 30px 0;
}

.home_insurance_list {
  width: 90%;
  margin: auto;
}

.home_insurance_list > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 27px;
  text-align: center;
  margin-bottom: 40px;
  color: #08374b;
}

.home_insurance_list > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: flex-start;
}

.home_insurance_list > div > div {
  width: 45%;
  border: 1px solid #08374b;
  box-sizing: border-box;
  border-radius: 12px;
  padding: 20px;
}

.home_insurance_list > div > div > div {
  width: 100px;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: flex-start;
}

.home_insurance_list > div > div > div > div {
  width: 40px;
  height: 40px;
  border-radius: 60px;
  overflow: hidden;
}

.home_insurance_list > div > div > h6 {
  font-style: normal;
  font-weight: bold;
  font-size: 11px;
  line-height: 17px;
  letter-spacing: -0.2px;
  color: #2a9d8f;
  margin-top: 20px;
}

.home_insurance_list > div > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 17px;
  letter-spacing: -0.2px;
  color: #272833;
  margin: 10px 0;
}

.home_insurance_list > div > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 17px;
  letter-spacing: -0.4px;
  color: #08374b;
}

.home_insurance_partner {
  width: 90%;
  margin: auto;
}

.home_insurance_partner > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 27px;
  text-align: center;
  color: #08374b;
  margin-top: 30px;
}

.home_insurance_partner_img {
  padding: 0 10px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  height: 100px;
}

.home_connect {
  background: #122933;
  padding: 30px 0 150px 0;
}

.home_connect > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 27px;
  text-align: center;
  color: #ffffff;
}

.home_connect > div {
  width: 80%;
  margin: auto;
}

.home_connect > div > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: flex-start;
  margin-top: 30px;
}

.home_connect > div > div > p {
  width: 35px;
  height: 35px;
  border-radius: 60px;
  background: #f3a627;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.home_connect > div > div > div {
  width: calc(100% - 50px);
}

.home_connect > div > div > div > h6 {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 22px;
  /* identical to box height */

  color: #ffffff;
}

.home_connect > div > div > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 18px;
  /* or 129% */
  margin-top: 10px;
  color: #ffffff;
}

.home_clinic {
  background: #fff;
}

.home_clinic > div {
  width: 90%;
  margin: auto;
  position: relative;
  height: 300px;
}

.home_clinic > div > div {
  position: absolute;
  top: -100px;
  left: 0;
  width: 100%;
  background: #fff2db;
  border-radius: 5px;
  padding: 50px 20px;
  text-align: center;
}

.home_clinic > div > div > img {
  width: 67px;
}

.home_clinic > div > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 27px;
  text-align: center;
  color: #090811;
  margin-top: 20px;
}

.home_clinic > div > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 24px;
  /* or 150% */
  margin: 20px 0;
  text-align: center;

  color: #000000;
}

.home_clinic > div > div > div {
  width: 217px;
  margin: auto;
  background: #f3a627;
  border-radius: 5px;
}

.home_clinic > div > div > div > a > div {
  height: 56px;

  font-style: normal;
  font-weight: bold;
  font-size: 13px;
  line-height: 18px;
  text-align: center;
  text-transform: uppercase;
  color: #122933;
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.home_clinic > div > div > div > a > div > svg {
  width: 10px;
  margin-right: 10px;
}

.home_power {
  background: #fff;
  padding: 20px 0 50px 0;
}

.home_power > div {
  width: 90%;
  margin: auto;
  padding: 0 20px;
}

.home_power > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 30px;
  /* or 150% */

  text-align: center;

  color: #000000;
  width: 250px;
  margin: auto;
}

.home_power > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 24px;
  /* or 150% */

  text-align: center;

  color: #000000;
  margin: 20px auto;
  max-width: 350px;
}

.home_power > div > div {
  width: 217px;
  margin: auto;
  background: #f3a627;
  border-radius: 5px;
}

.home_power > div > div > a > div {
  height: 55px;

  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 16px;

  text-align: center;
  text-transform: uppercase;

  color: #312828;

  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.home_video {
  background: #fff;

  padding: 20px;
}

.home_video > p {
  font-style: italic;
  font-weight: normal;
  font-size: 14px;
  line-height: 18px;
  /* or 129% */

  text-align: center;

  color: #122933;
}

.home_video > h5 {
  font-style: italic;
  font-weight: 600;
  font-size: 14px;
  line-height: 18px;
  /* identical to box height, or 129% */

  text-align: center;

  color: #122933;
  margin: 10px 0 5px 0;
}

.home_video > h6 {
  font-style: italic;
  font-weight: 600;
  font-size: 9px;
  line-height: 18px;
  /* identical to box height, or 200% */

  text-align: center;

  color: #122933;

  opacity: 0.6;
}

.home_video > div {
  background-image: url('~assets/images/banner/video.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  height: 172px;
  margin-bottom: 20px;
}

.home_video > div > div {
  width: 42px;
  height: 42px;
  background: #f3a627;
  border-radius: 60px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.home_rate {
  background: #f5f4ff;
  padding: 30px 20px;
}

.home_rate > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 27px;
  text-align: center;
  color: #000000;
}

.home_rate_list {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  margin-top: 30px;
}

.home_rate_list > svg {
  width: 20px;
}

.home_rate_para {
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 20px;
  text-align: center;
  letter-spacing: -0.1px;
  color: #000000;
  margin-top: 10px;
}

.home_rate_details {
  width: 200px;
  margin: 20px auto 0 auto;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
}

.home_rate_details > p {
  width: 43px;
  height: 43px;
}

.home_rate_details > div {
  width: calc(100% - 50px);
}

.home_rate_details > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  /* line-height: 28px; */
  /* identical to box height, or 200% */
  letter-spacing: -0.3px;
  color: #323232;
}

.home_rate_details > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  /* line-height: 28px; */
  letter-spacing: -0.3px;
  color: #323232;
  margin-top: 5px;
}
</style>
