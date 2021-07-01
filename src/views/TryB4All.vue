<template>
  <div class="home">
    <AppHeader v-bind="props" />
    <div class="login-form-frame">
      <div class="container">
        <div class="row">
          <div class="col-12 col-lg-6">
            <div class="content-login">
              <h2>
                Sign up to test our <br />
                IVR Call Centre
              </h2>
              <p>The call centre is currently operating using two numbers:</p>
              <h4>
                <p>
                  <span class="phone-call-frame mr-10"
                    ><img
                      src="../assets/images/phone-call-blue.png"
                      class="img-fluid"
                      alt="phone-call-blue"
                    />
                  </span>
                  <b>English (UK): </b><a href="tel:+441904803378">+44 1904 803378</a> / <a href="tel:+17372450200">+1 737 245 0200</a>
                </p>
                <p>
                  <span class="phone-call-frame mr-10"
                    ><img
                      src="../assets/images/phone-call-blue.png"
                      class="img-fluid"
                      alt="phone-call-blue"
                    /> </span
                  ><b>French (FR): </b> <a href="tel:+447723432543">+44 7723 432543</a>
                </p>
                <p>
                  <span class="phone-call-frame mr-10"
                    ><img
                      src="../assets/images/phone-call-blue.png"
                      class="img-fluid"
                      alt="phone-call-blue"
                    /> </span
                  ><b>Urdu (PK): </b> <a href="tel:+441485500402">+44 1485 500402</a>
                </p>
              </h4>
              <p>
                Follow the instructions to enrol using your voice print,
                enabling you to navigate through the use cases.
              </p>
              <p>
                If you would like to suggest a new use case to meet your
                business needs, contact the
                <a
                  href="https://www.gsma.com/mobilefordevelopment/mobile-money/gsma-inclusive-tech-lab/"
                  target="_blank"
                >
                  Inclusive Tech Lab</a
                >
                or
                <a @click="scrollBottom" class="link-color">
                  suggest a new use case.</a
                >
              </p>
            </div>
          </div>
          <div class="col-12 col-lg-6">
            <div class="sign-up-frame">
              <h2>Sign up</h2>
              <form @submit.prevent="processForm" method="post">
                <div class="form-group">
                  <label for="inputAddress">Nickname</label>
                  <input
                    type="text"
                    class="form-control"
                    id="inputAddress"
                    placeholder="Enter nickname"
                    v-model="nickName"
                  />
                  <span class="error-msg" v-if="errors.nickName.length != 0">
                    {{ errors.nickName }}</span
                  >
                </div>
                <div class="form-group">
                  <label for="inputAddress2">Mobile number</label>
                  <vue-tel-input
                    v-model="phone"
                    mode="international"
                    validCharactersOnly
                  ></vue-tel-input>
                  <span
                    class="error-msg"
                    v-if="errors.phone.length != 0 || errors.format.length != 0"
                  >
                    {{ errors.phone }} {{ errors.format }}
                  </span>
                </div>

                <div class="form-group">
                  <div class="form-check">
                    <label class="form-check-label">
                      <input
                        class="form-check-input"
                        type="checkbox"
                        id="gridCheck"
                        v-model="termsConditions"
                        true-value="yes"
                        false-value="no"
                      />
                      <span class="checkmark"></span>
                      <a href="./terms-and-condition.pdf" target="_blank"
                        >Accept the terms and conditions</a
                      >
                    </label>
                    <span class="error-msg" v-if="errors.tc.length != 0">
                      {{ errors.tc }}</span
                    >
                  </div>
                </div>

                <a v-if="showSubmit && !loading" href="#" class="btn1">
                  <input class="btn" type="submit" value="Submit Now" />
                </a>
                <b-spinner
                  style="margin-left: 45%"
                  v-if="loading"
                  label="Spinning"
                ></b-spinner>
                <div class="form-response" v-if="gotResponse">
                  <b-alert
                    variant="primary"
                    show
                    v-if="response.data.ResponseCode == 200"
                  >
                    {{ response.data.msg }}</b-alert
                  >
                  <b-alert
                    variant="danger"
                    show
                    v-if="response.data.ResponseCode == 623"
                  >
                    {{ response.data.msg }}</b-alert
                  >
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
    <section class="two-col-biometric-wrap text-white">
      <b-container>
        <b-row class="justify-content-start align-items-center">
          <b-col cols="12" xl="6">
            <div class="biometric-content">
              <h2>
                Test Different <br />
                Biometric Providers
              </h2>
              <p>
                Biometrics For All allows mobile money providers to test
                multiple biometrics solutions available in the market. Our
                solution was structured with a modular and flexible
                architecture, allowing new biometrics providers to include their
                solutions to showcase both in our IVR call centre and in the
                mobile app. Our team is constantly evolving the assets,
                increasing the range of possible suppliers available. If you are
                a biometric supplier and would like to contribute to our
                showcase, please
                <a
                  href="https://www.gsma.com/mobilefordevelopment/mobile-money/gsma-inclusive-tech-lab/"
                  target="_blank"
                >
                  contact the Inclusive Tech lab.</a
                >
              </p>
            </div>
          </b-col>
          <b-col cols="12" xl="6">
            <div class="biometric-img-block">
              <b-row
                class="justify-content-center align-items-center gutter-20 flex-md-column"
              >
                <b-col cols="12" md="7">
                  <a href="https://voiceit.io/" target="_blank">
                  <div class="bg-biometric2 bg-black">
                    <img
                      src="../assets/images/biometric-provide-icon-1.svg"
                      class="img-fluid"
                      alt="biometric-provide-icon-1"
                    />
                  </div>
                  </a>
                  <a href="https://diamondfortress.com/" target="_blank">
                  <div class="bg-biometric2 bg-blue">
                    <img
                      src="../assets/images/biometric-provide-icon-3.svg"
                      class="img-fluid"
                      alt="biometric-provide-icon-3"
                    />
                  </div>
                  </a>                  
                </b-col>
              </b-row>
            </div>
          </b-col>
        </b-row>
      </b-container>
    </section>
    <div class="about-content-wrapper try-frame">
      <div class="container">
        <div class="row">
          <div class="col-12 col-md-6">
            <div class="img-about-content">
              <img
                src="../assets/images/Guide.png"
                class="img-fluid"
                alt="Guide"
              />
            </div>
          </div>
          <div class="col-12 col-md-6">
            <h2>
              Use our documentation to get the most out of your experience
            </h2>
            <h6>
              B4LL allows you to experience different use cases. Our
              documentation guides you through happy and unhappy flows and tells
              you everything you need to know to make the correct use of the
              showcase. So please visit our documentation page and try to go
              over the flows which are outlined. There is an infinite number of
              open possibilities, so, help us to improve bringing your business
              needs so we can provide a customised experience to you.
            </h6>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Vue from "vue";
import axios from "axios";
import VueAxios from "vue-axios";
Vue.use(VueAxios, axios);
import AppHeader from "../components/AppHeader";
import Footer from "../components/layout/Footer";
import { VueTelInput } from "vue-tel-input";
export default {
  name: "TryB4All",
  components: { AppHeader, Footer, VueTelInput },
  data: () => ({
    props: {
      tittle: "EXPERIENCE THE BIOMETRICS SHOWCASE",
      breadCrumb: {
        tittle: "Try B4ll",
        link: "tryb4all",
      },
    },
    value: "",
    phone: "",
    nickName: "",
    termsConditions: "no",
    errors: {
      format: "",
      nickName: "",
      phone: "",
      tc: "",
    },
    showSubmit: true,
    loading: false,
    gotResponse: false,
    response: {},
  }),
  methods: {
    scrollBottom() {
      window.scrollTo({
        top: 10000,
        left: 0,
        behavior: "smooth",
      });
    },

    processForm(e) {
      this.errors = {
        format: "",
        nickName: "",
        phone: "",
        tc: "",
      };
      this.response = {};
      this.gotResponse = false;
      let noformat = true;
      const number = this.phone.split(" ").join("");
      if (number.length > 17 || number.length < 12) {
        noformat = false;
        this.errors.format = "Enter phone number in correct format.";
      }

      if (
        this.phone &&
        this.nickName &&
        this.termsConditions === "yes" &&
        noformat
      ) {
        this.loading = true;
        let postData = {
          Nickname: this.nickName,
          id: number,
        };

        this.axios
          .post(
            "https://6f0vqrhy90.execute-api.eu-west-2.amazonaws.com/dev/en-GB/webSignUp",
            postData,
            {
              headers: {
                "Content-Type": "application/json",
                "Access-Control-Allow-Origin": "*",
              },
            }
          )
          .then((res) => {
            this.loading = false;
            this.gotResponse = true;
            this.response = res;
            if (res.ResponseCode == 200) {
              this.showSubmit = false;
            }
          })
          .catch((err) => {
            this.loading = false;
            this.response = res;
          });
        return true;
      }
      if (!this.nickName) {
        this.errors.nickName = "Nick Name required.";
      }

      if (!this.phone) {
        this.errors.phone = "Phone required.";
      }

      if (this.termsConditions === "no") {
        this.errors.tc = "Accept terms and conditions.";
      }

      e.preventDefault();
    },
  },
};
</script>
<style src="vue-tel-input/dist/vue-tel-input.css"></style>
<style>
.coming-soon-frame h4 {
  margin-bottom: 0;
  color: #fff;
  padding-top: 10px;
}
.try-frame {
  padding-top: 90px;
  padding-bottom: 90px;
}
.login-form-frame {
  padding-top: 71px;
  padding-bottom: 70px;
  position: relative;
}
.login-form-frame::before {
  content: "";
  background-image: url("../assets/images/phone-call.png");
  position: absolute;
  left: 49px;
  top: 17px;
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
  width: 100px;
  height: 100px;
}
.login-form-frame::after {
  content: "";
  background-image: url("../assets/images/bg.png");
  position: absolute;
  right: -10px;
  top: -61px;
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
  width: 391px;
  height: 550px;
  z-index: -1;
}
.error-msg {
  font-size: 12px;
  color: red;
}
.form-control:focus {
  outline: none;
  box-shadow: none;
  border: 1px solid #95236c;
}
.login-form-frame .btn {
  width: 100%;
}
.mr-10 {
  margin-right: 10px;
}
.phone-call-frame img {
  margin-top: -7px;
}
.login-form-frame .content-login h4 {
  font-weight: bold;
  position: relative;
  /* padding-left: 35px; */
}
.login-form-frame .content-login p a {
  /* color: #000000; */
  font-size: 16px;
}
.biometric-content p a {
  color: #fff;
}
/* .biometric-content p a:hover,
.biometric-content p a {
  color: #ae52c4;
} */
.link-color:hover {
  color: #ae52c4;
  cursor: pointer;
}
/* .login-form-frame .content-login h4::before {
  content: "";
  position: absolute;
  background-image: url("../assets/images/phone-call-blue.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  left: 0;
  top: 0;
  bottom: 0;
  width: 25px;
  height: 25px;
} */
.login-form-frame .sign-up-frame p {
  font-size: 14px;
}

.login-form-frame .sign-up-frame h2,
.login-form-frame .sign-up-frame p {
  text-align: center;
}
.login-form-frame .sign-up-frame {
  background-color: #f9f9f9;
  border-radius: 18px;
  border: 1px solid #f2f2f2;
  width: 485px;
  /* height: 501px; */
  padding-left: 26px;
  padding-top: 34px;
  padding-right: 28px;
  padding-bottom: 51px;
}
::placeholder {
  font-size: 14px;
}
.login-form-frame .sign-up-frame .checkmark {
  position: absolute;
  top: 5px;
  margin-right: 5px;
  left: 0;
  border: 1px solid #979797;
  width: 14px;
  height: 14px;
}
.login-form-frame .content-login h4 a {
  color: #373737;
  font-size: 18px;
  font-weight: bold;
}
.login-form-frame .sign-up-frame .form-check {
  padding-left: 0;
}
.login-form-frame .sign-up-frame .checkmark:after {
  content: "";
  position: absolute;
  display: none;
}
.form-check-label {
  display: block;
  position: relative;
  padding-left: 35px;
  margin-bottom: 12px;
  cursor: pointer;
  font-size: 14px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.form-check-label input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
  height: 0;
  width: 0;
}
/* Show the checkmark when checked */
.form-check-label input:checked ~ .checkmark:after {
  display: block;
}

/* Style the checkmark/indicator */
.form-check-label .checkmark:after {
  left: 3px;
  top: 0px;
  width: 5px;
  height: 10px;
  border: solid #95236c;
  border-width: 0 3px 3px 0;
  /* background-color: #95236c; */
  -webkit-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  transform: rotate(45deg);
}
.form-response {
  text-align: center;
  margin-top: 20px;
}
@media only screen and (max-width: 1024px) {
  .login-form-frame .sign-up-frame {
    width: auto;
  }
  .login-form-frame::after {
    content: "";
    background-image: url("../assets/images/bg.png");
    position: absolute;
    right: 0;
    bottom: 0;
    top: auto;
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center;
    width: 224px;
    height: 330px;
    z-index: -1;
  }
}
@media only screen and (max-width: 767px) {
  .coming-soon-frame h4 {
    margin-bottom: 30px;
  }
}
</style>
