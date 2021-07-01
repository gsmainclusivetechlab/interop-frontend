<template>
  <div>
    <section class="app-downloading-wrapper">
      <div
        class="downloading-frame d-flex justify-content-center align-items-center"
      >
        <b-container>
          <b-row>
            <b-col cols="12">
              <h2>
                Ready? Test our IVR Call Centre and App Now!
              </h2>
              <h4 class="text-white">
                And keep your eyes peeled for new functionalities coming soon
              </h4>
              <p>
                <em>
                  Be the innovator in your market. Experience how mobile
                  biometrics can be used to facilitate seamless payments
                </em>
              </p>
              <!-- <ul>
                <li>
                  <a href="#">
                    <img
                      src="../../assets/images/ios.svg"
                      class="img-fluid"
                      alt=""
                  /></a>
                </li>
                <li>
                  <a href="#">
                    <img
                      src="../../assets/images/google.svg"
                      class="img-fluid"
                      alt=""
                  /></a>
                </li>
              </ul> -->
            </b-col>
          </b-row>
        </b-container>
      </div>
    </section>
    <div class="new-case-wrapper w-100 ">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <div class="news-frame bg-1">
              <div
                class="news-head d-flex  justify-content-md-between align-items-center"
              >
                <div class="newscase-headline">
                  <h2>Request a new use case</h2>
                  <p>
                    Can’t find your specific use case? Our team can support you
                    in the assessment of new use cases.
                  </p>
                </div>
                <div class="newscase-btn">
                  <a id="show-modal" href="/requestform" class="btn-newscase"
                    >Request Now</a
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <footer>
      <div class="footer-wrapper footer-bg">
        <b-container>
          <b-row class="justify-content-end align-items-center">
            <b-col cols="12" md="3">
              <div class="logo-main-footer">
                <a href="/">
                  <img
                    src="../../assets/images/Logol1img.jpg"
                    class="img-fluid"
                    alt="Logol1img"
                  />
                </a>
              </div>
            </b-col>
            <b-col cols="12" md="9">
              <div class="right-footer-content">
                <ul>
                  <li>
                    <img
                      src="../../assets/images/mail.svg"
                      class="img-fluid"
                      alt="mail"
                    /><a
                      href="mailto:inclusivetechlab@gsma.com?subject=I’m interested in Biometrics For All"
                      target="_blank"
                      >inclusivetechlab@gsma.com</a
                    >
                  </li>
                  <!--<li>
                    <img
                      src="../../assets/images/globe-icon.svg"
                      class="img-fluid"
                      alt="globe-icon"
                    />English
                    <img
                      src="../../assets/images/arrow-white.svg"
                      alt="Logo"
                      class="img-fluid"
                    />
                  </li>
                  <li>
                    <img
                      src="../../assets/images/help-circle.svg"
                      class="img-fluid"
                      alt="help-circle"
                    />Help
                  </li>-->
                </ul>
              </div>
            </b-col>
          </b-row>
          <b-row>
            <b-col cols="12">
              <hr />
              <div class="footer-bottom text-center">
                <div class="footer-navigation">
                  <ul>
                    <li>
                      <a href="/">Home </a>
                    </li>
                    <li>
                      <a href="/howitworks">How it works</a>
                    </li>
                    <li><a href="/tryb4all">Try B4LL</a></li>
                    <li>
                      <a
                        href=" https://docs.biometrics.gsmainclusivetechlab.io/ "
                        >Documentation</a
                      >
                    </li>
                    <li><a href="/about">About</a></li>
                    <li><a href="/faq">FAQs</a></li>
                  </ul>
                </div>
                <p class="copyright">
                  <span class="copy-text"
                    >Copyright
                    <span class="copy-img">
                      <img
                        src="../../assets/images/copyright-symbol.png"
                        class="img-fluid "
                        alt="copyright-symbol"
                      /> </span
                  ></span>

                  <span class="copy-dis"> 2021 GSMA.All right reserved</span>
                </p>
                <div class="scroll-top" v-on:click="scrollTop">
                  <img
                    src="../../assets/images/backtotop-arrow.svg"
                    class="img-fluid "
                    alt="backtotop-arrow"
                  />
                </div>
              </div>
            </b-col>
          </b-row>
        </b-container>
        <div class="img-footer-biometric">
          <img
            src="../../assets/images/footer-bg-image.svg"
            class="img-fluid"
            alt="footer-bg-image"
          />
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data: () => ({
    iframe: {
      source: "./requestForm.html",
      loaded: false,
    },
    showModal: false,
  }),

  methods: {
    scrollTop() {
      window.scrollTo({ left: 0, top: 0, behavior: "smooth" });
    },
  },

  watch: {
    $route(to, from) {
      this.modalClose();
    },
  },
};
</script>

<style>
ul {
  list-style: none;
}
.app-downloading-wrapper .downloading-frame {
  background-image: url("../../assets/images/woman-3083376_1920.png");
  min-height: 386px;
  text-align: center;
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  position: relative;
  display: flex;
  color: #fff;
  justify-content: center;
  align-items: center;
}
.app-downloading-wrapper .downloading-frame ul,
.os-system-wrap {
  display: block;
  padding-left: 0;
  margin: auto;
  text-align: center;
}
.app-downloading-wrapper .downloading-frame ul li,
.os-system-wrap ul li {
  display: inline-block;
  list-style-type: none;
  padding: 20px 0;
  padding-right: 10px;
}
.os-system-wrap ul li img {
  max-width: 100px;
}
.new-case-wrapper .news-frame {
  z-index: 9;

  color: #fff;
  border-radius: 5px;
  position: absolute;
  width: 100%;
  left: 0;
  right: 0;
  padding-top: 26px;
  padding-right: 26px;
  padding-bottom: 26px;
  padding-left: 29px;
  top: calc(100px - 157px);
}
.footer-wrapper .right-footer-content ul {
  padding-left: 0;
  padding-bottom: 0;
  margin-bottom: 0;
}

.bg-1 {
  background: #95236c;
}
*,
::after,
::before {
  box-sizing: border-box;
}
div {
  display: block;
}

.btn-newscase {
  color: #95236c;
  background: #fff;
  padding: 16px 30px;
  line-height: normal;
  border-radius: 5px;
  margin: 20px 10px;
  cursor: pointer;
}
.footer-wrapper .right-footer-content ul li img {
  padding-right: 5px;
}
.btn-newscase:hover {
  color: #95236c;
  text-decoration: none;
}
footer ul {
  display: block;
}
footer ul li,
footer ul li a {
  display: inline-block;
  list-style-type: none;
  font-size: 14px;
  line-height: normal;
  color: #fff;
}
footer p.copyright {
  font-size: 14px;
}
.footer-wrapper {
  min-height: 308px;
  position: relative;
  color: #fff;
  /* height: 308px; */
  justify-content: center;
  align-items: center;
  display: flex;
  padding-top: 65px;
}

/* .footer-wrapper .footer-headline {
  padding-top: 100px;
} */
.footer-wrapper .right-footer-content {
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
}
.footer-wrapper .right-footer-content ul li {
  list-style: none;
  padding: 20px 10px;
  display: inline-block;
  padding-bottom: 0;
  padding-right: 50px;
  padding-top: 0;
}
.footer-wrapper .right-footer-content ul li:last-child {
  padding-right: 0;
}
.footer-wrapper .footer-bottom ul li {
  padding: 20px 10px;
}
.footer-bottom .text-center {
  text-align: center !important;
}
.footer-bg {
  background: #181818;
}
*,
::after,
::before {
  box-sizing: border-box;
}
hr {
  background: #d8d8d8;
  margin-top: 1rem;
  margin-bottom: 1rem;
  border: 0;
  border-top: 1px solid #3c3c3c;
}
.footer-bottom {
  position: relative;
}
.footer-wrapper .img-footer-biometric {
  position: absolute;
  right: 0;
  bottom: 0;
}
.copyright img {
  margin-left: 5px;
  margin-right: 5px;
}
.scroll-top {
  position: absolute;
  right: 2px;
  top: 20px;
  border-radius: 5px;
  background: #95236c;
  width: 50px;
  height: 50px;
  line-height: 50px;
  z-index: 99;
}
.new-case-wrapper .newscase-headline p {
  padding-bottom: 0;
  margin-bottom: 0;
}
.new-case-wrapper .newscase-headline h2 {
  padding-bottom: 11px;
  margin-bottom: 0;
}
.copy-text {
  position: relative;
  padding-right: 17px;
}
.copy-img {
  content: "";
  width: 12px;
  height: 12px;
  background-image: url("../../assets/images/footer-bg-image.svg");
  background-size: contain;
  background-position: center;
  position: absolute;
  right: 8px;
  top: -6px;
  bottom: 0;
}

.footer-navigation ul {
  padding-left: 0;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.new-case-wrapper iframe {
  height: 100vh;
  width: 100vw;
  border: none;
  box-sizing: border-box;
}
.new-case-wrapper body {
  margin: 0;
}
.footer-wrapper .logo-main-footer img {
  width: 46px;
  height: 45px;
}
@media only screen and (max-width: 1024px) {
  .gsma-form .modal-container {
    width: 100%;
    height: 100%;
  }
  .gsma-form iframe {
    height: 75vh;
    width: 100%;
    border: none;
    box-sizing: border-box;
    margin-top: 21px;
  }
}
@media only screen and (min-width: 1200px) {
  .footer-wrapper .container {
    max-width: 1171px;
  }
}
@media only screen and (max-width: 993px) {
  .footer-wrapper {
    padding-top: 167px;
  }

  .scroll-top {
    position: absolute;
    right: 0;
    left: 0;
    top: auto;
    text-align: center;
    bottom: 20px;
    margin: auto;
  }
  .footer-bottom {
    padding-bottom: 75px;
  }
  .footer-wrapper .footer-bottom ul li {
    display: list-item;
  }
  .news-head {
    flex-wrap: wrap;
  }
  .news-head .newscase-headline {
    margin-bottom: 30px;
    width: 100%;
    text-align: center;
  }
  .new-case-wrapper .newscase-btn {
    width: 100%;
    text-align: center;
  }
}
@media only screen and (max-width: 767px) {
  .footer-navigation ul {
    display: block;
  }
  .footer-wrapper .footer-bottom ul li {
    padding-bottom: 0;
  }
  .footer-wrapper {
    padding-top: 189px;
  }
  .footer-wrapper .logo-main-footer {
    margin: auto;
    text-align: center;
    margin-bottom: 10px;
  }
  .footer-wrapper .right-footer-content ul {
    margin: auto;
    text-align: center;
  }
  .footer-wrapper .right-footer-content ul li {
    padding-left: 0;
    margin-bottom: 15px;
    padding-right: 0;
  }
  .footer-wrapper .right-footer-content ul li:first-child {
    width: 100%;
  }
  .footer-wrapper .right-footer-content ul li:nth-of-type(2) {
    padding-right: 37px;
  }
  .new-case-wrapper .news-frame {
    text-align: center;
    margin: 0 15px;
    width: auto;
  }

  .new-case-wrapper .news-frame {
    top: calc(100% - 132px);
  }
}
</style>
