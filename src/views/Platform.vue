<template>
  <div class="home">
    <AppHeader v-bind="props" />

    <!-- SECTION 01: The ITP -->
    <section class="bio-all">
      <div class="container">
        <div class="bio-all-contents">
          <div class="row">
            <div class="col-12 col-lg-6">
              <div class="bio-content-wrap">
                <h2>The Interoperability Test Platform</h2>
                <p>
                  The GSMA's Interoperability Test Platform is the first joint end-to-end test environment to test interoperable 
                  mobile money solutions, including joining two key technologies, the <a href="https://www.gsma.com/mobilefordevelopment/mobile-money/mobile-money-api/"
                target="_blank">GSMA Mobile Money API</a> and <a href="https://mojaloop.io/" target="_blank"> the Mojaloop.</a> 
                  With this test platform, the GSMA provides the industry with an open-source and secure environment, enabling 
                  ecosystem participants to test their systems across different use cases.
                </p>
                <p>
                  The test platform links two key technologies in the mobile money industry; first, the GSMA Mobile Money API, 
                  which provides a modern harmonised API for mobile money transactions and management, enabling seamless 
                  integration between service providers and mobile money operators, and second, the Gates Foundation’s Mojaloop, 
                  open-source software to operate a financial hub.
                </p>
              </div>
            </div>
            <div class="col-12 col-lg-6">
              
              <div class="row">
                <img
                  src="../assets/images/laptop.png"
                  class="img-fluid"
                  alt="usecase-content"
                />
              </div>
              <div  class="row center">
              <p>
                <a href="http://interop.gsmainclusivetechlab.io/" target="_blank" text-align="center" class="btn">Access the Platform</a>
              </p>
            </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- SECTION 02: How The ITP Works -->
    <section class="two-col-biometric-wrap text-white managing-content">
      <div class="container">
        <div class="row">
          <div class="col-12 col-lg-6">
            <div class="right-manage-img">
              <h2 class="mb-0">How does the ITP works?</h2>
                <p>
                  The ITP makes the work of testing platform connections much easier and simple. It is based on plug-and-play solutions. 
                </p>
                
                  <div class="twoline-managing-frame">
                    <div class="img-manage">
                      <img
                        src="../assets/images/feature-icon-9.png"
                        class="img-fluid"
                        alt="feature-icon-1"
                      />
                    </div>
                    <div class="content-manage-frame">
                      <h5>1. Select the type of test and the system under test </h5>
                      <p>
                        The sessions can be manually customised, or the platform suggests the tests based on a quick questionnaire.
                      </p>
                    </div>
                  </div>

                  <div class="twoline-managing-frame">
                    <div class="img-manage">
                      <img
                        src="../assets/images/feature-icon-10.png"
                        class="img-fluid"
                        alt="feature-icon-1"
                      />
                    </div>
                    <div class="content-manage-frame">
                      <h5>2. Define the Use Cases and Test Cases</h5>
                      <p>
                        The test cases to validate the SUT can be assessed using both happy and unhappy flows. Each test case follows a template which makes easier to replicate, maintain and create new ones.
                      </p>
                    </div>
                  </div>  

                  <div class="twoline-managing-frame">
                    <div class="img-manage">
                      <img
                        src="../assets/images/feature-icon-11.png"
                        class="img-fluid"
                        alt="feature-icon-1"
                      />
                    </div>
                    <div class="content-manage-frame">
                      <h5>3. Run each test case and check the results.</h5>
                      <p>
                        Running the test cases the user can analyse all the package (header and body) exchanged during the transactions. This allows a better understand of the information in case of run failures. 
                      </p>
                    </div>
                  </div>  
              
            </div>
          </div>
          <div class="col-12 col-lg-1"></div>
          <div class="col-12 col-lg-5">
            <div class="row">
                <img
                  src="../assets/images/itp-interface.png"
                  class="img-fluid"
                  alt="usecase-content"
                />
              </div>
          </div>
          
        </div>
      </div>
    </section>

    <!-- Section 3: ON Boarding and Certification -->
    <div class="mobile-app-content grey-bg">
      <div class="container">
        <div class="row">
          <div class="col-12 col-lg-5">
            <div>
              <img
                src="../assets/images/NewGraphic-interoperability-02.png"
                class="img-fluid"
                alt="mobile-app"
              />
            </div>
          </div>
          <div class="col-12 col-lg-7">
            <div class="app-content-wrap">
              <h2>On-boarding and Certification</h2>
              <h6>
               Interoperability hub operators face many challenges when onboarding new participants. To maintain the overall health of the network, it is critical to ensure that new participants follow correct processes with respect to the interoperability protocol. The main focus was on supporting the operators with the many challenges faced during the onboarding and certification process. 
              </h6>
              <h6>
                Therefore, any interested mobile operator or service provider can customise the available code to ensure that new participants follow the correct processes with respect to the interoperability protocol. For this, we provide documentation and direct support from our team to assist during the customisation process. All material is available on a page about the interoperability potential and how the Inclusive Tech Lab's technical assets can help speed up the testing and integration process.
              </h6>
            </div>
          </div>
          
        </div>
      </div>
    </div>

    <section class="tutorial-section text-center">
      <div class="container">
        <div class="row">
          <div class="col-12">
          <h2>Customise your solution</h2>
            <p>
              The modular architecture of ITP encompasses a large number of elements and covers the entire end-to-end mobile money transaction ecosystem. This means that each module of the platform's code can be customised to meet the desired needs. This is one of the great potentials of ITP. In addition, we can also isolate a subset of modules for restricted testing, covering a specific part of the entire interoperability ecosystem. 
            </p>
            <!-- <img src="../assets/images/Call.png" class="img-fluid" alt="Call" /> -->
          </div>
        </div>
      </div>
    </section> 
    <Footer />
  </div>
</template>

<script>
import AppHeader from "../components/AppHeader";
import Footer from "../components/layout/Footer";
export default {
  name: "HowItWorks",
  components: { AppHeader, Footer },
  data: () => ({
    props: {
      tittle: "INSIDE THE INTEROPERABILITY TEST PLATFORM",
      breadCrumb: {
        tittle: "How it works",
        link: "/howitworks",
      },
    },
  }),
};
</script>

<style>
.card-wrap h5 {
  font-weight: bold;
}
.center{
  display: flex;
  justify-content: center;
}
.card-wrap {
  background-color: #ffffff;
  box-shadow: 0 16px 40px rgba(0, 0, 0, 0.1);
  min-height: 249px;
  border-radius: 10px;
  padding-top: 35px;
  padding-left: 25px;
  padding-bottom: 28px;
  padding-right: 25px;
  transition: all 0.25s ease-out;
  height: calc(100% - 30px);
  margin-bottom: 30px;
}
.card-wrap img {
  padding-bottom: 25px;
}
.managing-content {
  padding-top: 64px;
  padding-bottom: 94px;
}
.managing-content h2 {
  margin-bottom: 40px;
}
.twoline-managing-frame {
  display: flex;
  justify-content: flex-start;
}
.twoline-managing-frame .img-manage {
  padding-right: 21px;
}
.twoline-managing-frame .img-manage img {
  max-width: 41px;
}
.tutorial-section {
  position: relative;
  padding-top: 71px;
  padding-bottom: 73px;
}
.tutorial-section p {
  padding-bottom: 35px;
}
.tutorial-section::before {
  content: "";
  position: absolute;
  left: 0;
  background-image: url(../assets/images/bio-left.svg);
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
  top: 0;
  bottom: 0;
  width: 169px;
  left: 0;
}
.tutorial-section::after {
  content: "";
  position: absolute;
  right: 0;
  background-image: url(../assets/images/video-bg-1.svg);
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
  width: 400px;
  height: 290px;
  bottom: 0;
}
.usecase-wrapper {
  padding-top: 40px;
  padding-bottom: 77px;
}
.usecase-wrapper .usecase-main {
  padding-bottom: 55px;
}
.usecase-wrapper .usecase-three-col-content .usecase-frame {
  background-color: #ffffff;
  border-radius: 8px;
  box-shadow: 0 2px 23px rgba(0, 0, 0, 0.13);
  min-height: 104px;
  padding-top: 19px;
  padding-left: 16px;
  padding-right: 45px;
  padding-bottom: 11px;
  margin-bottom: 37px;
}
.usecase-wrapper .usecase-three-col-content .usecase-frame .usecase-img {
  width: 50px;

  margin-right: 20px;
}
.usecase-wrapper .usecase-three-col-content .usecase-frame .usecase-img img {
  max-width: 41px;
}
.grey-bg {
  background-color: #f3f3f3;
}
.mobile-app-content {
  padding-top: 68px;
  position: relative;
}
.mobile-app-content::after {
  content: "";
  /* background-image: url("../assets/images/dots.png"); */
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  position: absolute;
  min-height: 291px;
  top: 0;
  left: 0;
  width: 345px;
}
.mobile-app-content .app-content-wrap {
  padding-bottom: 113px;
}
.mobile-app-content .img-app-wrap {
  position: absolute;
  width: 686px;
  height: 501px;
  bottom: -106px;
  left: 0;
}
.usecase-wrapper {
  position: relative;
}
.usecase-wrapper::before {
  content: "";
  background-position: center;
  background-image: url("../assets/images/Bubble-small.png");
  background-repeat: no-repeat;
  background-size: contain;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 259px;
  height: 261px;
}
.usecase-wrapper .usecase-three-col-content::after {
  content: "";
  background-position: center;
  background-image: url("../assets/images/bubblel.png");
  background-repeat: no-repeat;
  background-size: contain;
  position: absolute;
  top: -127px;
  right: 0;
  width: 280px;
  height: 443px;
  display: block;
  z-index: -1;
}
.usecase-wrapper .usecase-three-col-content {
  position: relative;
}
.bio-all {
  padding-top: 77px;
  position: relative;
  padding-bottom: 85px;
}

.bio-all::after {
  content: "";
  background-image: url("../assets/images/bg-3.png");
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

@media only screen and (max-width: 993px) {
  .card-wrap {
    margin-bottom: 30px;
  }
  .right-manage-img {
    margin: auto;
    text-align: center;
  }
}
@media only screen and (max-width: 767px) {
  .tutorial-section::after {
    width: 150px;
    height: 111px;
  }
}
</style>
