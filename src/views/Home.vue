<template>
  <div class="home">
    
    <div class="home-header">
      <NavBar />
      <div class="slider-portfolio">
        <b-carousel
          id="carousel-no-animation"
          style="text-shadow: 0px 0px 2px #000"
          no-animation
          indicators
          img-width="1024"
          img-height="480"
        >
          <b-carousel-slide>
            <!-- <b-container> -->
            <h1>MOBILE MONEY</h1>
            <h1>INTEROPERABILITY</h1>
            <div class="biometric-content-carousal">
              <h4> Supporting the Industry to Accelerate </h4>
              <h4> Open and Interconnected Payment Systems </h4>
              <div class="os-system-wrap">
                <ul>
                  <li>
                    <a href="http://interop.gsmainclusivetechlab.io/" target="_blank">
                    <img
                      src="../assets/images/download-itp.png"
                      class="img-fluid"
                      alt="Access the ITP"
                    />
                    </a>
                  </li>
                  <li>
                    <a href="https://compliance.mobilemoneyapi.io/login" target="_blank">
                    <img
                      src="../assets/images/download-compliance.png"
                      class="img-fluid"
                      alt="Access the Compliance Platform"
                    />
                    </a>
                  </li>
                </ul>
              </div>
            </div>
            <!-- </b-container> -->
            
            <template #img>
              <div>
                <img
                class="img-fluid slider-img"
                width="1024"
                height="480"
                src="../assets/images/NewGraphic-interoperability-01.png"
                alt="image slot"
                />
              </div>
            </template>
            
          </b-carousel-slide>
        </b-carousel>
      </div>
    </div>
    
    <!-- FRAME 01: INTRODUCTION -->
    <div class="digital-wrapper grey-bg">
      <b-container>
        <b-row>
          <b-col cols="12" md="6">
            <div class="digital-frame-left-content">
              <h3>
                Mobile Money Interoperability
              </h3>
              <p>
                In the world of mobile money, interoperability has been one of the industry’s north stars for years, as it holds the promise of an interconnected 
                world in which people in emerging markets can send money to each other regardless of the mobile money service they are using. 
              </p>
              
              <p>
                For over a decade, mobile money has been driving financial inclusion, opening access to digital transactions and giving people the tools 
                to better manage their financial lives. The rapid rise of the mobile money industry has been accompanied by an increasing emphasis on the need for account-to-account interoperability.
            </p>
            <p></p>
            </div>
          </b-col>
          <b-col cols="12" md="1"></b-col>
          <b-col cols="12" md="5">
            <div class="content-digital">
              <h4> Are you a mobile operator or financial services provider looking to provide interoperability in emerging markets?</h4>
              <h4> Check what the Interoperability Test Platform can do for you!</h4>
              <div  class="row center">
                <p>
                  <a href="https://itp.gsmainclusivetechlab.io"  class="btn btn-lap">Read more</a>
                </p>
            </div>
            </div>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <!-- FRAME 02: LAPTOP -->
    <section class="bio-all ">
      <div class="container">
        <div class="bio-all-contents">
          <div class="row">
            <div class="col-12 col-lg-6">
              <div class="bio-content-wrap">
                <h2>Connecting Financial Products</h2>
                <p>
                  Interoperability refers to the ability to make an electronic money transfer between two accounts held at different institutions. 
                </p>
                <p>
                  In the context of mobile money, the term interoperability can be used in many ways, but the simplest use case is for mobile money providers to give customers the ability to transfer money between two accounts in different mobile money schemes, or between accounts at a mobile money scheme and a bank, known as account-to-account (A2A) interoperability.
                </p>
                <p>
                  Interoperable payment systems can connect customers, merchants, banks and other financial service providers, creating an open, harmonised ecosystem and providing greater financial inclusion.
                </p>
              </div>
            </div>
            <div class="col-12 col-lg-6">
              <div class="img-bio">
                <img
                  src="../assets/images/NewGraphic-interoperability-03.png"
                  class="img-fluid"
                  alt="usecase-content"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    
    <!-- FRAME 03: PROBLEMS -->
    <section class="two-col-biometric-wrap text-white">
      <b-container>
        <b-row class="justify-content-start align-items-center">
          
          <b-col cols="12" xl="5">
            <div class="biometric-img-block">
              <img
                  src="../assets/images/NewGraphic-interoperability-04.png"
                  class="img-fluid"
                  alt="usecase-content"
                />
            </div>
          </b-col>
          <b-col cols="12" xl="1"></b-col>
          <b-col cols="12" xl="6">
            <div class="biometric-content">
              <h2>
                Many Paths to Mobile Money Interoperability
              </h2>
              <p>
                Mobile money interoperability has been implemented differently in different markets and contexts. The technical solutions deployed have been diverse, reflecting differences in scope and ambition, as well as evolving standards and regulations. While mobile money interoperability is not new, most solutions are still in their infancy.
              </p>
              <p>
                This is why the Inclusive Tech Lab created an open-source platform to help industry players to evaluate different technologies, develop interoperable solutions, and provide onboarding and certification capabilities for an interconnected world. 
              </p>
            </div>
          </b-col>
          
        </b-row>
      </b-container>
    </section>

    
    <div class="digital-wrapper feature-wrap bg-greys">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <div class="feature-content text-center">
              <h2> A Technological Blueprint</h2>
              <h6>
                How to make your products interoperable?
              </h6>
            </div>
            <div class="three-col-feature-frame">
              <div class="row justify-content-center">
                <div class="col-12 col-md-6 col-lg-4">
                  <div class="card-wrap">
                    <img
                      src="../assets/images/icon_world.png"
                      class="img-fluid"
                      alt="development"
                    />
                    <h5>Common technologies and standards</h5>
                    <h6>
                      Industry alignment on standards and technical specifications.
                    </h6>
                  </div>
                </div>
                <div class="col-12 col-md-6 col-lg-4">
                  <div class="card-wrap">
                    <img
                      src="../assets/images/icon_government.png"
                      class="img-fluid"
                      alt="trusted"
                    />
                    <h5>Platform and integration tools</h5>
                    <h6>
                      Enabling digital finance service providers to test relevant use cases and ensure they are ready to go for production.
                    </h6>
                  </div>
                </div>
                <div class="col-12 col-md-6 col-lg-4">
                  <div class="card-wrap">
                    <img
                      src="../assets/images/icon_app.png"
                      class="img-fluid"
                      alt="smartphones"
                    />
                    <h5>Onboarding and certification process</h5>
                    <h6>
                      Schemes to ensure high-quality processes, and reliability, and security.
                    </h6>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    
    <!-- FRAME FAQ -->
    <!-- <section class="question-wrapper">
      <b-container>
        <b-row>
          <b-col cols="12">
            <div class="headline-accordion-wrap text-center bg-dark-color ">
              <h2>Frequently Asked Questions</h2>
            </div>

            <div class="accordion" role="tablist">
              <b-card no-body class="card-header mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button
                    block
                    v-b-toggle.accordion-1
                    variant="light"
                    class="card-link"
                    >I want to showcase my biometric solution on B4LL. How can I do that?</b-button
                  >
                </b-card-header>
                <b-collapse
                  id="accordion-1"
                  visible
                  accordion="my-accordion"
                  role="tabpanel"
                >
                  <b-card-body>
                    <b-card-text
                      >We are always happy to engage with new partners. If you think you have a biometric solution that may be suitable to be showcased through B4LL, please get in touch with us.</b-card-text
                    >
                  </b-card-body>
                </b-collapse>
              </b-card>

              <b-card no-body class="card-header mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button
                    block
                    v-b-toggle.accordion-2
                    variant="light"
                    class="card-link"
                    >Is the GSMA ITL providing biometric verification solutions through B4LL commercially?</b-button
                  >
                </b-card-header>
                <b-collapse
                  id="accordion-2"
                  accordion="my-accordion"
                  role="tabpanel"
                >
                  <b-card-body>
                    <b-card-text
                      >No, B4LL is a completely free facility. The solutions housed within B4LL are not commercial offerings from the GSMA ITL. If service providers like the general experience of the solutions housed within B4LL, they are free to adopt them commercially in their markets. The GSMA ITL would not be privy to any such commercial adoption of biometric solutions by service providers. </b-card-text
                    >
                  </b-card-body>
                </b-collapse>
              </b-card>

              <b-card no-body class="card-header mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button
                    block
                    v-b-toggle.accordion-3
                    variant="light"
                    class="card-link"
                    >Is it possible to see the call centre working in a different languages or dialects?</b-button
                  >
                </b-card-header>
                <b-collapse
                  id="accordion-3"
                  accordion="my-accordion"
                  role="tabpanel"
                >
                  <b-card-body>
                    <b-card-text
                      >Sure! You can have the call centre working in any language or dialect, or even multiple languages.</b-card-text
                    >
                  </b-card-body>
                </b-collapse>
              </b-card>
            </div>
            <div class="questions-frame text-center">
              <p>
                Still have a question?<span class="question-bold">
                  <a href="#"> Ask your question here</a></span
                >
              </p>
            </div>
          </b-col>
        </b-row>
      </b-container>
    </section> -->
    <Footer />
  </div>
</template>

<script>
import NavBar from "../components/layout/NavBar";
import Footer from "../components/layout/Footer";
export default {
  name: "Home",
  components: { NavBar, Footer },
};
</script>
<style>
.home-header {
  background-image: linear-gradient(180deg, #02568D 0%, #424985 100%);
}
.home-header::before {
  content: "";
  background-image: url("../assets/images/banner-bg-gradient.png");
  background-position: top;
  position: absolute;
  top: 2px;
  left: 0;
  width: 421px;
  height: 625px;
  background-repeat: no-repeat;
}
.slider-portfolio {
  min-height: 511px;
  position: relative;
}
.slider-portfolio .carousel-item {
  z-index: 9;
}
.slider-portfolio::after {
  content: "";
  background-image: url("../assets/images/dots.png");
  background-position: top;
  position: absolute;
  bottom: 0;
  right: 0;
  width: 365px;
  height: 270px;

  z-index: 0;
  background-repeat: no-repeat;
}
.slider-portfolio .carousel-item img {
  height: fit-content;
  object-fit: contain;
  object-position: right;
  padding-top: 135px;
  float: right;
  padding-top: 0px;
  padding-right: 14px;
}
.slider-portfolio .carousel-control-next-icon,
.slider-portfolio .carousel-control-prev-icon {
  display: none;
}
.slider-portfolio .carousel-indicators {
  justify-content: flex-start;
  margin-left: 108px;
  bottom: 63px;
}
.slider-portfolio .carousel-indicators li:focus,
.slider-portfolio .carousel-indicators li.active {
  outline: none;
  border: none;
}
.carousel-caption {
  position: absolute;
  right: 0;
  bottom: 80px;
  left: 0;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: left;

  margin-left: 108px;
}
.slider-portfolio .carousel-caption h1,
.slider-portfolio .carousel-caption h4 {
  color: #ffffff;
}
.slider-portfolio .carousel-indicators li {
  background-color: rgba(255, 255, 255, 0.33);
  border-radius: 50%;
  width: 10px;
  height: 10px;
  border-top: none;
  border-bottom: none;
}
.slider-portfolio .carousel-indicators li.active {
  background-color: #ffffff;
  border-radius: 5px;
  width: 28px;
  height: 10px;
}

.slider-portfolio .os-system-wrap ul {
  padding-left: 0;
}
.slider-portfolio .os-system-wrap {
  display: block;
  padding-left: 0;
  margin: auto;
  text-align: left;
  position: relative;
}
/* .slider-portfolio .os-system-wrap .img-soon{
  position: absolute;
      bottom: 9px;
      top: 0;
}
.slider-portfolio .os-system-wrap  span.img-soon img {
    max-width: 90px;
    height: auto;
    margin-top: -16px;
} */

.slider-portfolio .os-system-wrap ul li {
  display: inline-block;
  list-style-type: none;
  padding: 20px 0;
}

.slider-portfolio .os-system-wrap ul li img {
  max-width: 230px;
}
.digital-wrapper {
  padding: 82px 0;
  padding-bottom: 0;
}
.digital-wrapper h4 {
  padding-bottom: 40px;
  margin-bottom: 0;
}
.digital-wrapper .full-width-banner h4 {
  padding-bottom: 30px;
}
.mobile-group-banner {
  background-image: url("../assets/images/group10.png");
  min-height: 621px;
  background-size: contain;
  background-repeat: no-repeat;
  background-position: center;
  margin-bottom: -201px;
  z-index: 0;
}
.digital-wrapper {
  position: relative;
}
.full-width-banner {
  padding-top: 60px;
  padding-bottom: 32px;
}
/*.digital-wrapper::before {
  content: "";
  background-image: url("../assets/images/biometric-bg-icon-2.png");
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  position: absolute;
  width: 243px;
  height: 232px;
  left: 11px;
  top: 36px;
}*/
/* .digital-wrapper::after {
  content: "";
  background-image: url("../assets/images/biometric-bg-icon-1.png");
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  position: absolute;
  right: 0;
  bottom: 0;
  width: 141px;
  height: 135px;
} */

.two-col-biometric-wrap {
  min-height: 556px;
  background-image: linear-gradient(180deg, #02568D 0%, #424985 100%);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  z-index: 1;
  position: relative;
}
.two-col-biometric-wrap .biometric-img-block {
  display: flex;
  justify-content: center;
  align-items: center;
}
.two-col-biometric-wrap .bg-biometric,
.two-col-biometric-wrap .bg-biometric2,
.two-col-biometric-wrap .bg-biometric3 {
  justify-content: center;
  display: flex;
  align-items: center;
  margin: auto;
  border-radius: 10px;
  position: relative;
}
.two-col-biometric-wrap .bg-biometric {
  width: 100%;
  min-width: 188px;
  min-height: 188px;
}
.two-col-biometric-wrap .bg-biometric2,
.two-col-biometric-wrap .bg-biometric3 {
  width: 160px;
  min-width: 160px;
  min-height: 163px;
  /* height: 163px; */
  padding: 10px;
  margin-top: 20px;
  /* margin-right: 20px; */
}
.two-col-biometric-wrap .bg-biometric3.bg-blue {
  margin-left: 20px;
}
.two-col-biometric-wrap .bg-biometric::before {
  content: "";
  /*background-image: url("../assets/images/biometric-bg-icon-2.png");*/
  background-image: url("../assets/images/dots-01.png");
  position: absolute;
  background-position: center;
  background-size: contain;
  left: -132px;
  top: -47px;
  background-repeat: no-repeat;
  width: 150px;
  min-height: 150px;
  z-index: -1;
}
.two-col-biometric-wrap .bg-biometric2::before {
  content: "";
  /*background-image: url("../assets/images/biometric-bg-icon-2.png");*/
  background-image: url("../assets/images/dots-01.png");
  position: absolute;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  right: 128px;
  top: -54px;
  width: 150px;
  min-height: 150px;
  z-index: -1;
}
.two-col-biometric-wrap .bg-biometric3::before {
  content: "";
  background-image: url("../assets/images/biometric-bg-icon-3.png");
  position: absolute;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  left: 105px;
  bottom: -71px;
  width: 150px;
  min-height: 150px;
  z-index: -1;
}
.mb-20 {
  margin-bottom: 20px !important;
}
.bg-black {
  background: #000000;
}
.bg-white {
  background: #ffff;
}
.bg-blue {
  background: #1f2747;
}
.row.gutter-20 {
  margin-left: -10px;
  margin-right: -10px;
}
.row.gutter-20 [class*="col-"] {
  padding-left: 10px;
  padding-right: 10px;
}
.two-col-biometric-wrap .biometric-right-col {
  background-image: url("../assets/images/dots-01.png");
  display: flex;
  justify-content: center;
  align-items: flex-start;
  flex-direction: row;
  height: 100%;
}
.card-header {
  background-color: transparent !important;
}
.card-header p-1 {
  display: block;
  padding: 16px 20px;
  padding-right: 35px;
  font-size: 16px;
  color: #000;
  font-weight: 700;
}
.accordion .card .card-header {
  padding: 0;
  border-bottom: 0;
  background: transparent;
}
.accordion .card {
  border: none;
  border-bottom: 1px solid #cccccc !important;
  padding: 0;
}
.accordion .card .card-body p {
  margin-bottom: 0;
}

.question-bold a {
  font-weight: 700;
  color: #00568D;
  padding-left: 10px;
}
.question-wrapper {
  padding: 40px 0;
}
.question-wrapper .btn-light:hover {
  color: transparent;
  background-color: transparent;
  border-color: transparent;
}
.question-wrapper .btn.focus,
.btn:focus {
  box-shadow: none;
}
.questions-frame {
  padding: 40px 0;
}
.question-wrapper .headline-accordion-wrap {
  padding: 10px 0;
}
.accordion .card .card-header .card-link {
  display: block;
  padding: 16px 20px;
  padding-right: 35px;
  font-size: 16px;
  color: #000;
  font-weight: 700;
  background: transparent;
  border: none;
  text-align: left;
  padding-left: 0;
}
.accordion .card .card-body {
  padding-top: 0;
  padding-left: 0;
}

.accordion .card .card-header .card-link[aria-expanded="true"] {
  color: #00568D;
}
.accordion .card .card-header .card-link .collapsed > .when-opened {
  color: #00568D;
  content: "";
  background-image: url("../assets/images/accordion-arrow-active.svg");
}

.accordion .card .card-header .card-link.collapsed > .when-opened,
:not(.collapsed) > .when-closed::after {
  content: "";
  background-image: url("../assets/images/accordion-arrow-active.svg");
}
.accordion .card .card-header .card-link::after {
  content: "";
  position: absolute;
  background-image: url("../assets/images/accordion-arrow.svg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  width: 20px;
  height: 20px;
  line-height: 20px;
  right: 15px;
  top: 21px;
  display: block;
  transition: transform 0.3s cubic-bezier(0.455, 0.03, 0.515, 0.955);
}
.content-digital p {
  color: #000000;
}
.accordion .btn-light:not(:disabled):not(.disabled).active:focus,
.accordion .btn-light:not(:disabled):not(.disabled):active:focus,
.accordion .show > .btn-light.dropdown-toggle:focus,
.accordion .card .card-header .card-link.active {
  outline: none;
  box-shadow: none;
  border: none;
}
.accordion .card .card-header .card-link[aria-expanded="true"]::after {
  content: "";
  background-image: url("../assets/images/accordion-arrow-active.svg");
}
.card-link .btn-light:hover {
  color: #fdfdfe;
  background-color: transparent;
  border-color: transparent;
}

.bio-all {
  padding-top: 77px;
  position: relative;
  padding-bottom: 85px;
}

.bio-all::after {
  content: "";
  /* background-image: url("../assets/images/dots-01.png"); */
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  width: 400px;
  height: 350px;
  position: absolute;
  top: 0;
  right: 0;
  z-index: -1;
}
.bio-all .img-bio {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  height: 100%;
}
.bio-all .img-bio img {
  margin-left: 85px;
}
@media only screen and (max-width: 1024px) {
  .bio-all .img-bio img {
    margin-left: 0;
  }
  .tutorial-section::after {
    width: 250px;
    height: 185px;
  }
  .mobile-app-content .img-app-wrap {
    position: relative;
    width: 100%;
    height: auto;
    bottom: 0;
    left: 0;
    right: 0;
    margin: auto;
    margin-bottom: 20px;
  }
}

.btn{
  background-color: #00A5C7;
  border-radius: 6px;
  min-width: 155px;
  min-height: 50px;
  color: #fff;
  padding: 10px;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  font-size: 16px;
}
.btn:hover {
  background-color: #025e89;
  border-radius: 6px;
  min-width: 155px;
  min-height: 50px;
  color: #fff;
  padding: 10px;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  font-size: 16px;
}
.digital-wrapper.feature-wrap {
  padding-top: 58px;
}
.digital-wrapper.feature-wrap .feature-content h2 {
  margin-bottom: 0;
  padding-bottom: 16px;
}
.feature-wrap .three-col-feature-frame {
  padding-top: 41px;
  padding-bottom: 97px;
}
@media only screen and (min-width: 1025px) {
  .slider-img {
    width: 650px;
    height: 471px !important;
  }
}
@media only screen and (max-width: 1204px) {
  .two-col-biometric-wrap {
    padding-top: 40px;
    padding-bottom: 40px;
  }
}
@media only screen and (max-width: 1024px) {
  .carousel-caption {
    bottom: 100px;
  }
  .slider-portfolio .carousel-indicators {
    margin-left: 69px;
  }
  .slider-portfolio .carousel-caption {
    margin-left: 69px;
  }
  .home-header::before {
    height: 505px;
  }
  .slider-img {
    width: 400px;
    height: 400px !important;
  }
  .slider-portfolio {
    min-height: 400px;
  }

  .questions-frame {
    padding-bottom: 0;
  }
}
@media only screen and (max-width: 993px) {
  .mobile-group-banner {
    min-height: 450px;
    background-size: contain;
  }

  .slider-portfolio .os-system-wrap ul li {
    padding-bottom: 0;
    padding-top: 15px;
  }
  .biometric-content-carousal {
    display: none;
  }
}
@media only screen and (min-width: 768px) {
  .btn-mob {
    display: none;
  }
}
@media only screen and (max-width: 767px) {
  .two-col-biometric-wrap .biometric-right-col {
    flex-direction: column;
  }
  .two-col-biometric-wrap .bg-biometric3.bg-blue {
    margin-left: 0;
  }
  .two-col-biometric-wrap .bg-biometric2,
  .two-col-biometric-wrap .bg-biometric3 {
    margin-top: 0;
    margin-bottom: 30px;
  }
  .digital-wrapper::before {
    width: 150px;
    height: 200px;
    left: -4px;
    top: -18px;
  }
  .digital-wrapper::after {
    display: none;
  }
  .mobile-group-banner {
    min-height: 220px;
  }
  .mobile-group-banner {
    margin-bottom: -64px;
  }
  .app-downloading-wrapper .downloading-frame ul,
  .os-system-wrap {
    display: inline-flex;
  }
  .app-downloading-wrapper .downloading-frame {
    padding: 30px 0;
    padding-bottom: 150px;
  }

  .two-col-biometric-wrap .bg-biometric,
  .two-col-biometric-wrap .bg-biometric2,
  .two-col-biometric-wrap .bg-biometric3 {
    min-height: 145px;
    margin-bottom: 30px;
    width: 100%;
  }
  .btn-lap {
    display: none;
  }
  .slider-img {
    width: 300px;
    height: 269px !important;
    margin: auto;
    text-align: center;
  }
  .slider-portfolio .carousel-caption {
    right: 0;
    text-align: center;
    left: 0;
    bottom: -69px;
    margin: auto;
  }
  .slider-portfolio .carousel-indicators {
    margin: auto;
    justify-content: center;
    bottom: 43px;
  }
  .slider-portfolio .carousel-item img,
  .slider-portfolio .carousel-item {
    float: none;
    text-align: center;
    margin: auto;
  }
  .slider-portfolio .carousel.pointer-event,
  .slider-portfolio .carousel-inner {
    min-height: 400px;
  }
}
@media only screen and (max-width: 480px) {
  .home-header::before {
    height: 400px;
    width: 100%;
  }
  .slider-portfolio::after {
    width: 100%;
    height: 156px;
  }
}

</style>
