<template>
  <div class="cover_list">
    <div>
      <div>
        <div class="cover_list_img">
          <div>
            <div>
              <img src="@/assets/images/lady.png" alt="" />
            </div>
            <div>
              <img src="@/assets/images/lagos.png" alt="" />
            </div>
          </div>
        </div>
        <div class="cover_list_details">
          <h6>INDIVIDUAL COVER</h6>
          <p>The Lagos State Health Scheme</p>
          <h3>N8,500</h3>
          <h5>
            <nuxt-link to="/all-available-insurance/individual"
              ><span>VIEW DETAILS</span> &#8594;</nuxt-link
            >
          </h5>
        </div>
      </div>
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
.cover_list {
  background: #fff;
}

.cover_list > div > div {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
  padding: 20px;
}

.cover_list_img {
  width: 45%;
  max-width: 130px;
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
}
</style>
