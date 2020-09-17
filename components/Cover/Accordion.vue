<template>
  <div class="cover_div">
    <div>
      <div class="cover_div_header" @click="selectedCover = 'services'">
        <p>Services Covered</p>
        <div>+</div>
      </div>
      <div class="cover_div_body" v-if="selectedCover === 'services'">
        <div>
          <h3>About this insurance</h3>
          <p>
            The Lagos State Health Scheme is a mandatory state-wide health
            scheme that will give your dependent access to basic, better-quality
            healthcare services for one whole year. Both private as public
            clinics are accessible through the scheme.
          </p>
        </div>
      </div>
    </div>
    <div>
      <div class="cover_div_header" @click="selectedCover = 'quality'">
        <p>Ensuring Quality Care</p>
        <div>+</div>
      </div>
      <div class="cover_div_body" v-if="selectedCover === 'quality'">
        <div>
          <h3>About this insurance</h3>
          <p>
            The Lagos State Health Scheme is a mandatory state-wide health
            scheme that will give your dependent access to basic, better-quality
            healthcare services for one whole year. Both private as public
            clinics are accessible through the scheme.
          </p>
        </div>
      </div>
    </div>
    <div>
      <div class="cover_div_header" @click="selectedCover = 'hospitals'">
        <p>Available Hospitals</p>
        <div>+</div>
      </div>
      <div class="cover_div_body" v-if="selectedCover === 'hospitals'">
        <div>
          <h3>About this insurance</h3>
          <p>
            The Lagos State Health Scheme is a mandatory state-wide health
            scheme that will give your dependent access to basic, better-quality
            healthcare services for one whole year. Both private as public
            clinics are accessible through the scheme.
          </p>
        </div>
      </div>
    </div>
    <div>
      <div class="cover_div_header" @click="selectedCover = 'works'">
        <p>How it works</p>
        <div>+</div>
      </div>
      <div class="cover_div_body" v-if="selectedCover === 'works'">
        <div>
          <h3>About this insurance</h3>
          <p>
            The Lagos State Health Scheme is a mandatory state-wide health
            scheme that will give your dependent access to basic, better-quality
            healthcare services for one whole year. Both private as public
            clinics are accessible through the scheme.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedCover: '',
    }
  },
}
</script>

<style scoped>
.cover_div {
  width: 90%;
  margin: auto;
  background: #fafefd;
  padding: 5px 20px;
}

.cover_div > div {
  margin: 20px 0;
}

.cover_div_header {
  background: #08374b;
  border-radius: 2px;
  height: 60px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  padding: 0 20px;
}

.cover_div_header > p {
  width: calc(100% - 10px);
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 24px;
  color: #fafefd;
}

.cover_div_header > div {
  width: 10px;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 24px;
  color: #fafefd;
}

.cover_div_body {
  padding: 10px 0;
}

.cover_div_body > div {
  background: #ffffff;
  border: 0.87287px solid #2a9d8f;
  box-sizing: border-box;
  border-radius: 2px;
  padding: 30px 20px;
}

.cover_div_body > div > h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 24px;
  color: #08374b;
}

.cover_div_body > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 20px;
  color: rgba(0, 0, 0, 0.56);
  margin-top: 10px;
}
</style>
