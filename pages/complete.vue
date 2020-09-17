<template>
  <div class="complete_div">
    <Header />
    <div class="complete_div_thank">
      <div>
        <svg
          width="21"
          height="16"
          viewBox="0 0 21 16"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M6.67368 12.6234L1.69528 7.64802L0 9.33035L6.67368 16L21 1.68233L19.3167 0L6.67368 12.6234Z"
            fill="#F3A627"
          />
        </svg>
      </div>
      <h3>Thank you!</h3>
      <p>Your payment was successful!</p>
      <p>
        A payment confirmation has been sent to your email ayo@acumen.com.ng
      </p>
    </div>
    <div class="complete_div_share">
      <div class="complete_div_share_arrow">
        <svg
          width="16"
          height="16"
          viewBox="0 0 16 16"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M7.29289 0.292893C6.90237 0.683418 6.90237 1.31658 7.29289 1.70711L12.5858 7H1C0.447715 7 0 7.44772 0 8C0 8.55229 0.447715 9 1 9H12.5858L7.29289 14.2929C6.90237 14.6834 6.90237 15.3166 7.29289 15.7071C7.68342 16.0976 8.31658 16.0976 8.70711 15.7071L15.7064 8.70782C15.7088 8.70541 15.7112 8.70298 15.7136 8.70055C15.8901 8.52079 15.9992 8.27463 16 8.003C16 8.002 16 8.001 16 8C16 7.999 16 7.998 16 7.997C15.9996 7.8625 15.9727 7.73425 15.9241 7.61722C15.8764 7.50195 15.8063 7.3938 15.7136 7.29945C15.7112 7.29705 15.7089 7.29466 15.7065 7.29228M15.7065 7.29228L8.70711 0.292893C8.31658 -0.0976311 7.68342 -0.0976311 7.29289 0.292893"
            fill="#F3A627"
          />
        </svg>
      </div>
      <h3>Next Steps</h3>
      <p>
        Inform your primary member to complete their registration so they can
        start accessing care.
      </p>
      <div class="complete_div_share_whatapp">
        <p>Share Link via Whatsapp</p>
        <div>
          <img src="@/assets/images/whatsapp.svg" alt="" />
        </div>
      </div>
      <div class="complete_div_share_email">
        <p>Share Link via Email</p>
        <div><img src="@/assets/images/mail.svg" alt="" /></div>
      </div>
      <div class="complete_div_share_sms">
        <p>Share Link via SMS</p>
        <div><img src="@/assets/images/sms.svg" alt="" /></div>
      </div>
    </div>
    <div class="complete_div_chat">
      <p>
        If your primary member does not have a smartphone, please chat with us.
      </p>

      <div class="complete_div_share_chat">
        <p>Chat with us</p>
        <div><img src="@/assets/images/chat.svg" alt="" /></div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from '@/components/HeaderEmpty'

export default {
  components: {
    Header,
  },
  data() {
    return {}
  },
}
</script>

<style scoped>
.checkout_div {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #ffffff;
  overflow: auto;
  padding-bottom: 100px;
}

.complete_div_thank {
  padding-top: 50px;
  padding-bottom: 30px;
  padding-left: 20px;
  padding-right: 20px;
  margin: auto;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
}

.complete_div_thank > div {
  width: 42px;
  height: 42px;
  border-radius: 60px;
  background: rgba(243, 166, 39, 0.2);
  margin: auto;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.complete_div_thank > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 28px;
  line-height: 40px;
  text-align: center;
  color: #000000;
  margin-top: 20px;
}

.complete_div_thank > p {
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 24px;
  text-align: center;
  color: rgba(0, 0, 0, 0.67);
  opacity: 0.9;
  margin: 10px 0;
}

.complete_div_share {
  padding-top: 50px;
  padding-bottom: 30px;
  padding-left: 20px;
  padding-right: 20px;
  margin: auto;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
}

.complete_div_share_arrow {
  width: 42px;
  height: 42px;
  border-radius: 60px;
  background: rgba(243, 166, 39, 0.2);
  margin: auto;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-content: center;
  align-items: center;
}

.complete_div_share > h3 {
  font-style: normal;
  font-weight: bold;
  font-size: 28px;
  line-height: 40px;
  text-align: center;
  color: #000000;
  margin-top: 20px;
}

.complete_div_share > p {
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 24px;
  text-align: center;
  color: rgba(0, 0, 0, 0.67);
  opacity: 0.9;
  margin: 10px 0;
}

.complete_div_share_whatapp {
  background: #1bd741;
  border-radius: 5px;
  margin: auto;
  height: 58px;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex;
  align-content: center;
  align-items: center;
  padding: 0 20px;
  margin-top: 20px;
  position: relative;
}

.complete_div_share_whatapp > p {
  width: calc(100% - 58px);
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 24px;
  color: #ffffff;
}

.complete_div_share_whatapp > div {
  width: 50px;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-end;
  align-content: center;
  align-items: center;
}

.complete_div_share_whatapp > div > img {
  width: 25px;
}

.complete_div_share_email {
  background: #122933;
  border-radius: 5px;
  margin: auto;
  height: 58px;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex;
  align-content: center;
  align-items: center;
  padding: 0 20px;
  margin-top: 20px;
  position: relative;
}

.complete_div_share_email > p {
  width: calc(100% - 58px);
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 24px;
  color: #ffffff;
}

.complete_div_share_email > div {
  width: 50px;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-end;
  align-content: center;
  align-items: center;
}

.complete_div_share_email > div > img {
  width: 25px;
}

.complete_div_share_sms {
  background: #2a9d8f;
  border-radius: 5px;
  margin: auto;
  height: 58px;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex;
  align-content: center;
  align-items: center;
  padding: 0 20px;
  margin-top: 20px;
  position: relative;
}

.complete_div_share_sms > p {
  width: calc(100% - 58px);
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 24px;
  color: #ffffff;
}

.complete_div_share_sms > div {
  width: 50px;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-end;
  align-content: center;
  align-items: center;
}

.complete_div_share_sms > div > img {
  width: 25px;
}

.complete_div_chat {
  padding-top: 50px;
  padding-left: 20px;
  padding-right: 20px;
  margin: auto;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
  padding-bottom: 100px;
}

.complete_div_chat > p {
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 24px;
  text-align: center;
  color: rgba(0, 0, 0, 0.67);
  opacity: 0.9;
  margin: 10px 0;
}

.complete_div_share_chat {
  background: #f3a627;
  border-radius: 5px;
  margin: auto;
  height: 58px;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex;
  align-content: center;
  align-items: center;
  padding: 0 20px;
  margin-top: 20px;
  position: relative;
}

.complete_div_share_chat > p {
  width: calc(100% - 58px);
  font-style: normal;
  font-weight: normal;
  font-size: 17px;
  line-height: 24px;
  color: #ffffff;
}

.complete_div_share_chat > div {
  width: 50px;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-end;
  align-content: center;
  align-items: center;
}

.complete_div_share_chat > div > img {
  width: 25px;
}
</style>
