<template>
  <div class="website_letter">
    <div>
      <h3>Stay informed with us</h3>
      <h6>Subscribe to our newsletter</h6>
      <div>
        <input type="text" placeholder="Your email" />
        <button>subscribe</button>
      </div>
      <p>We will never share your information with a third-party.</p>
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
.website_letter {
  padding: 30px 0;
  background: #fafefd;
}

.website_letter > div {
  width: 90%;
  margin: auto;
}

.website_letter > div > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 17px;
  line-height: 23px;
  text-align: center;
  color: #122933;
}

.website_letter > div > h6 {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 19px;
  text-align: center;
  color: #122933;
}

.website_letter > div > div {
  max-width: 300px;
  margin: 20px auto 5px auto;
  background: #f5f4ff;
  box-sizing: border-box;
  border-radius: 2.5898px;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  overflow: hidden;
}

.website_letter > div > div > input {
  width: calc(100% - 100px);
  border: 1px solid #f3a627;
  font-style: normal;
  font-weight: normal;
  font-size: 11.6541px;
  line-height: 18px;
  color: #122933;
  height: 44px;
  outline: 0;
  padding: 0 5px;
}

.website_letter > div > div > button {
  width: 100px;
  height: 44px;
  font-style: normal;
  font-weight: 500;
  font-size: 9.0643px;
  line-height: 11px;
  letter-spacing: 1.2949px;
  text-transform: uppercase;
  color: #122933;
  background: #f3a627;
  outline: 0;
  border: 0;
  text-align: center;
}

.website_letter > div > p {
  font-style: normal;
  font-weight: normal;
  font-size: 10px;
  line-height: 14px;
  text-align: center;
  color: #122933;
  opacity: 0.4;
}
</style>
