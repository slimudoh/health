<template>
  <div>
    <div class="clinics_header">
      <div>
        <div>
          <img src="@/assets/images/clinic.svg" alt="" />
        </div>
        <h3>Find Available Clinics</h3>
        <p>
          Your family has a choice who they want as their preferred health
          provider.
        </p>
      </div>
    </div>

    <div class="clinics_search">
      <div>
        <div class="clinics_search_input">
          <div>
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g opacity="0.4">
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M16.2691 15.3937C17.2772 14.1885 17.884 12.6362 17.884 10.9422C17.884 7.1084 14.776 4 10.942 4C7.108 4 4 7.1084 4 10.9422C4 14.776 7.108 17.8845 10.942 17.8845C12.5291 17.8845 13.9918 17.3518 15.1611 16.4555L18.708 19.7922C19.017 20.0816 19.502 20.0672 19.792 19.7587C20.082 19.4501 20.067 18.9653 19.759 18.6749L16.2691 15.3937ZM10.942 16.3514C7.955 16.3514 5.533 13.93 5.533 10.9422C5.533 7.9555 7.955 5.5331 10.942 5.5331C13.93 5.5331 16.351 7.9555 16.351 10.9422C16.351 13.93 13.93 16.3514 10.942 16.3514Z"
                  fill="white"
                />
              </g>
            </svg>
          </div>

          <input type="text" placeholder="Search Clinic " />
        </div>
        <div class="clinics_search_search">
          <div>
            Sort by
            <svg
              width="9"
              height="6"
              viewBox="0 0 9 6"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M1.52588e-05 1.27138C0.00260925 1.3092 0.0022974 1.31882 0.0087347 1.35626C0.0232668 1.44045 0.0551739 1.52142 0.102051 1.59286C0.125739 1.62899 0.153303 1.66052 0.182711 1.69202L3.93287 5.44219C3.96059 5.46806 3.9669 5.47528 3.99719 5.49825C4.03119 5.52403 4.06785 5.54631 4.10641 5.56466C4.27489 5.64479 4.4748 5.64479 4.64328 5.56466C4.68184 5.54631 4.7185 5.52403 4.7525 5.49825C4.78275 5.47528 4.7891 5.46806 4.81678 5.44219L8.56695 1.69202C8.59282 1.6643 8.60007 1.65796 8.62301 1.62771C8.68329 1.54827 8.72398 1.45451 8.74095 1.35626C8.75302 1.2861 8.75302 1.214 8.74095 1.14384C8.73126 1.08775 8.71389 1.03303 8.68945 0.981619C8.5966 0.78636 8.404 0.650417 8.18893 0.628291C8.10393 0.619572 8.01736 0.628479 7.93592 0.654324C7.86807 0.675856 7.80404 0.709013 7.74735 0.752015C7.71707 0.774985 7.71075 0.782204 7.68303 0.80808L4.37483 4.11628L1.06662 0.80808L1.03543 0.778954C1.00606 0.755047 0.999215 0.748234 0.967463 0.72742C0.907961 0.688387 0.841802 0.659636 0.772674 0.642792C0.717359 0.629323 0.660232 0.623447 0.603354 0.625385C0.387252 0.63276 0.185836 0.755266 0.0798626 0.943711C0.0449858 1.00575 0.0208292 1.07372 0.0087347 1.14384C0.0022974 1.18128 0.00260925 1.19091 1.52588e-05 1.22872C1.52588e-05 1.24294 1.52588e-05 1.25716 1.52588e-05 1.27138Z"
                fill="#1A3947"
              />
            </svg>
          </div>
        </div>
      </div>
    </div>

    <div class="clinics_list">
      <div>
        <div>
          <div @click="details()">
            <div class="clinics_list_map">
              <img src="@/assets/images/map.png" alt="" />
            </div>
            <div class="clinics_list_details">
              <h6>Government Owned</h6>
              <h3>Alimosho Hospital Complex</h3>
              <p>12, Minna street, Charity B/Stop, Ipaja-Abesan, Lagos.</p>
            </div>
          </div>
          <div @click="details()">
            <div class="clinics_list_map">
              <img src="@/assets/images/map.png" alt="" />
            </div>
            <div class="clinics_list_details">
              <h6>Government Owned</h6>
              <h3>Alimosho Hospital Complex</h3>
              <p>12, Minna street, Charity B/Stop, Ipaja-Abesan, Lagos.</p>
            </div>
          </div>
          <div @click="details()">
            <div class="clinics_list_map">
              <img src="@/assets/images/map.png" alt="" />
            </div>
            <div class="clinics_list_details">
              <h6>Government Owned</h6>
              <h3>Alimosho Hospital Complex</h3>
              <p>12, Minna street, Charity B/Stop, Ipaja-Abesan, Lagos.</p>
            </div>
          </div>
          <div @click="details()">
            <div class="clinics_list_map">
              <img src="@/assets/images/map.png" alt="" />
            </div>
            <div class="clinics_list_details">
              <h6>Government Owned</h6>
              <h3>Alimosho Hospital Complex</h3>
              <p>12, Minna street, Charity B/Stop, Ipaja-Abesan, Lagos.</p>
            </div>
          </div>
          <div @click="details()">
            <div class="clinics_list_map">
              <img src="@/assets/images/map.png" alt="" />
            </div>
            <div class="clinics_list_details">
              <h6>Government Owned</h6>
              <h3>Alimosho Hospital Complex</h3>
              <p>12, Minna street, Charity B/Stop, Ipaja-Abesan, Lagos.</p>
            </div>
          </div>
          <div @click="details()">
            <div class="clinics_list_map">
              <img src="@/assets/images/map.png" alt="" />
            </div>
            <div class="clinics_list_details">
              <h6>Government Owned</h6>
              <h3>Alimosho Hospital Complex</h3>
              <p>12, Minna street, Charity B/Stop, Ipaja-Abesan, Lagos.</p>
            </div>
          </div>
        </div>
        <p><span>SEE MORE</span> &#8594;</p>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Footer from '@/components/Footer'

export default {
  components: {
    Footer,
  },
  methods: {
    details() {
      this.$router.push('/all-available-clinics/alimosho-clinic')
    },
  },
}
</script>

<style>
.clinics_header {
  background: #fff;
  padding: 30px 0;
}

.clinics_header > div {
  width: 90%;
  margin: auto;
}

.clinics_header > div > div {
  width: 50px;
  margin: auto;
}

.clinics_header > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 27px;
  text-align: center;
  color: #090811;
  margin: 10px 0;
}

.clinics_header > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 24px;
  text-align: center;
  color: #000000;
  opacity: 0.6;
  max-width: 300px;
  margin: auto;
}

.clinics_search {
  padding: 15px 0;
  background: #08374b;
}

.clinics_search > div {
  width: 80%;
  margin: auto;
  background: transparent;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.clinics_search_input {
  width: calc(100% - 100px);
  position: relative;
}

.clinics_search_input > div {
  position: absolute;
  top: 0;
  left: 0;
  width: 35px;
  height: 35px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.clinics_search_input > input {
  width: 100%;
  height: 35px;
  padding-left: 35px;
  padding-right: 5px;
}

.clinics_search_search {
  width: 100px;

  background: #f3a627;
  border-radius: 2px;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 24px;
  color: #1a3947;
}

.clinics_search_search > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  height: 35px;
}

.clinics_search_search > div > svg {
  width: 10px;
  margin-left: 5px;
}

.clinics_list {
  background: #e5e5e5;
  padding: 30px 0;
}

.clinics_list > div {
  width: 90%;
  margin: auto;
}

.clinics_list > div > div {
  margin-bottom: 50px;
}

.clinics_list > div > div > div {
  background: #fafefd;
  border-radius: 11px;
  padding: 20px;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  margin-bottom: 30px;
}

.clinics_list_map {
  width: 60px;
  height: 60px;
  background: #ebeaf4;
  border-radius: 4px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.clinics_list_map > img {
  width: 32px;
}

.clinics_list_details {
  width: calc(100% - 100px);
}

.clinics_list_details > h6 {
  font-style: normal;
  font-weight: normal;
  font-size: 9px;
  line-height: 18px;
  text-transform: uppercase;
  color: #2a9d8f;
}

.clinics_list_details > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
  letter-spacing: -0.2px;
  color: #272833;
  margin: 5px 0;
}

.clinics_list_details > p {
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 16px;
  color: #374a48;
}

.clinics_list > div > p {
  font-style: normal;
  font-weight: bold;
  font-size: 12px;
  line-height: 16px;
  text-transform: uppercase;
  color: #f3a627;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.clinics_list > div > p > span {
  width: 70px;
  text-decoration-line: underline;
}
</style>
