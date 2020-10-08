<template>
  <div>
    <Header />
    <div class="clinics_details">
      <div>
        <h6>
          <nuxt-link to="/all-available-clinics">
            &#8592; <span>go back</span>
          </nuxt-link>
        </h6>
        <div>
          <div class="clinics_details_txt">
            <h6>Government Owned</h6>
            <h3>Alimosho Hospital Complex</h3>
            <p>12, Minna street, Charity B/Stop, Ipaja-Abesan, Lagos.</p>
          </div>
          <div class="clinics_details_share">
            <div>
              <svg
                width="20"
                height="21"
                viewBox="0 0 20 21"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M12.6 14.5091C13.2682 13.8409 14.2227 13.3636 15.2727 13.3636C17.3727 13.3636 19.0909 15.0818 19.0909 17.1818C19.0909 19.2818 17.3727 21 15.2727 21C13.1727 21 11.4545 19.2818 11.4545 17.1818C11.4545 16.9909 11.4784 16.8239 11.5023 16.6568C11.5261 16.4898 11.55 16.3227 11.55 16.1318L6.49091 13.1727C5.82273 13.8409 4.86818 14.3182 3.81818 14.3182C1.71818 14.3182 0 12.6 0 10.5C0 8.4 1.71818 6.68182 3.81818 6.68182C4.86818 6.68182 5.82273 7.15909 6.49091 7.82727L11.6455 4.86818C11.6291 4.80267 11.6127 4.73998 11.5968 4.67912L11.5968 4.67911C11.5201 4.38529 11.4545 4.13449 11.4545 3.81818C11.4545 1.71818 13.1727 0 15.2727 0C17.3727 0 19.0909 1.71818 19.0909 3.81818C19.0909 5.91818 17.3727 7.63636 15.2727 7.63636C14.2227 7.63636 13.2682 7.15909 12.5045 6.49091L7.44546 9.45C7.46183 9.51551 7.47821 9.57821 7.4941 9.63906C7.57085 9.93289 7.63636 10.1837 7.63636 10.5C7.63636 10.6909 7.6125 10.858 7.58864 11.025C7.56477 11.192 7.54091 11.3591 7.54091 11.55L12.6 14.5091ZM17.1818 3.81818C17.1818 2.76818 16.3227 1.90909 15.2727 1.90909C14.2227 1.90909 13.3636 2.76818 13.3636 3.81818C13.3636 4.86818 14.2227 5.72727 15.2727 5.72727C16.3227 5.72727 17.1818 4.86818 17.1818 3.81818ZM3.81818 12.4091C2.76818 12.4091 1.90909 11.55 1.90909 10.5C1.90909 9.45 2.76818 8.59091 3.81818 8.59091C4.86818 8.59091 5.72727 9.45 5.72727 10.5C5.72727 11.55 4.86818 12.4091 3.81818 12.4091ZM13.3636 17.1818C13.3636 18.2318 14.2227 19.0909 15.2727 19.0909C16.3227 19.0909 17.1818 18.2318 17.1818 17.1818C17.1818 16.1318 16.3227 15.2727 15.2727 15.2727C14.6045 15.2727 13.9364 15.6545 13.65 16.2273C13.4591 16.5136 13.3636 16.8 13.3636 17.1818Z"
                  fill="#F3A627"
                />
              </svg>
            </div>
            <p>SHARE</p>
          </div>
        </div>
        <p>
          Open In GoogleMaps
          <svg
            width="8"
            height="8"
            viewBox="0 0 8 8"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M6.66667 2.27614L1.13807 7.80474C0.877722 8.06509 0.455612 8.06509 0.195262 7.80474C-0.0650874 7.54439 -0.0650874 7.12228 0.195262 6.86193L5.72386 1.33333H0.666667C0.298477 1.33333 0 1.03486 0 0.666667C0 0.298477 0.298477 0 0.666667 0H7.33333C7.42373 0 7.50992 0.0179903 7.58852 0.0505858C7.66715 0.083119 7.74082 0.131344 7.80474 0.195262C7.86866 0.25918 7.91688 0.332847 7.94941 0.411478C7.98201 0.490082 8 0.576273 8 0.666667V7.33333C8 7.70152 7.70152 8 7.33333 8C6.96514 8 6.66667 7.70152 6.66667 7.33333V2.27614Z"
              fill="#F3A627"
            />
          </svg>
        </p>
      </div>
    </div>

    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'

export default {
  components: {
    Header,
    Footer,
  },
}
</script>

<style scoped>
.clinics_details {
  background: #fff;
  padding: 30px 0;
}

.clinics_details > div {
  width: 90%;
  margin: auto;
}

.clinics_details > div > h6 {
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 16px;
  text-transform: uppercase;
  color: #f3a627;
}

.clinics_details > div > h6 > a > span {
  text-decoration-line: underline;
}

.clinics_details > div > p {
  font-style: normal;
  font-weight: bold;
  font-size: 13px;
  line-height: 30px;
  text-decoration-line: underline;
  color: #f3a627;
  text-align: center;
}

.clinics_details > div > p > svg {
  width: 10px;
}

.clinics_details > div > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  margin: 50px 0;
}

.clinics_details_share {
  width: 50px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.clinics_details_share > div {
  width: 37px;
  height: 37px;
  background: #ecdcc0;
  border-radius: 8px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.clinics_details_share > div > svg {
  width: 20px;
  height: 20px;
}

.clinics_details_share > p {
  font-style: normal;
  font-weight: bold;
  font-size: 10px;
  line-height: 14px;
  text-align: center;
  text-transform: uppercase;
  color: #2e383d;
}

.clinics_details_txt {
  width: calc(100% - 100px);
}

.clinics_details_txt > h6 {
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 18px;
  color: #2a9d8f;
}

.clinics_details_txt > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 30px;
  color: #08374b;
  margin: 10px 0;
}

.clinics_details_txt > p {
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 18px;
  color: #6e8e8a;
}
</style>
