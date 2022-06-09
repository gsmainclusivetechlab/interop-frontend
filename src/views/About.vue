<template>
  <div class="home">
    <AppHeader v-bind="props" />
    
    <!-- Section 01: Inclusive Tech Lab -->
    <div class="about-content-wrapper">
      <div class="container">
        <div class="row">
          
          <div class="col-12 col-md-6">
            <div class="img-about-content">
              <img
                src="../assets/images/bg-6.png"
                class="img-fluid"
                alt="Tech-lab"
              />
            </div>
          </div>
          
          <div class="col-12 col-md-6">
            <h2> </h2>
            <h6>
              The
              <a
                href="https://www.gsma.com/mobilefordevelopment/mobile-money/gsma-inclusive-tech-lab/"
                target="_blank"
              >
                GSMA Inclusive Tech Lab</a
              >
              supports the mobile money industry to develop the mobile financial
              ecosystem, to enable a broad range of digital transactions and
              make mobile wallets central to the lives of the financially
              excluded and underserved, providing them with better solutions to
              manage their financial resources and face economic shocks. Mobile
              money has evolved to a platform of more than 1 billion accounts
              reaching emerging market consumers and bringing financial access
              to the previously underserved and excluded. The Inclusive Tech Lab
              has published a set of harmonised Mobile Money Application
              Programming Interfaces (APIs) and is now looking at expanding the
              potential of mobile money through the use of biometrics for
              financial transactions.
            </h6>
          </div>
          
        </div>
      </div>
    </div>

    <section class="about-content-wrapper grey-bg">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <div class="bio-all-content-wrap">
              <h2>Mobile Money Interoperability</h2>
            </div>
          </div>
          <div class="col-12 col-lg-6">
            <div class="bio-all-content-wrap">
              <h6>
                In the world of mobile money, interoperability has been one of the industry’s north stars for years, 
                as it holds the promise of an interconnected world in which people in emerging markets can send money 
                to each other regardless of the mobile money service they are using. The mobile money industry is moving 
                in the direction of interoperability, however, support by and the independent facilitation of the GSMA is 
                often sought. Within this scenario, the Lab opens a dedicated workstream to support the industry.
              </h6>
              <h6>
                
              </h6>
              
            </div>
          </div>
          <div class="col-12 col-lg-6">
            <div class="img-bio-content">
              <h6>
                The GSMA’s Interoperability Test Platform is the first joint end-to-end test environment 
                to test interoperable mobile money solutions, including joining two key technologies, 
                the GSMA Mobile Money API and the Mojaloop. With this test platform, the GSMA provides 
                the industry with an open-source and secure environment, enabling ecosystem participants 
                to test their systems across different use cases.
              </h6>
            </div>
          </div>
        </div>
      </div>
    </section>
    <div class="contact-us-wrap">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <h2>
              Contact us to support you to pilot a <br />
              project in your market
            </h2>
            <a
              href="mailto:inclusivetechlab@gsma.com?subject=I’m interested in Biometrics For All"
              target="_blank"
              class="btn"
              >Contact</a
            >
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>
<script>
import AppHeader from "../components/AppHeader";
import Footer from "../components/layout/Footer";
export default {
  name: "About",
  components: { AppHeader, Footer },
  data: () => ({
    props: {
      tittle: "ABOUT",
      breadCrumb: {
        tittle: "About",
        link: "about",
      },
    },
  }),
};
</script>
<style>
.about-content-wrapper {
  padding-top: 63px;
  padding-bottom: 68px;
}
.about-content-wrapper .img-about-content {
  margin: auto;
  text-align: center;
  margin-top: -45px;
}
.contact-us-wrap {
  padding-top: 62px;
  padding-bottom: 71px;
  margin: auto;
  text-align: center;
  position: relative;
}
.contact-us-wrap::after {
  content: "";
  background-image: url("../assets/images/dots.png");
  background-position: center;
  background-size: contain;
  position: absolute;
  right: 0;
  top: 0;
  height: 300px;
  width: 367px;
  background-repeat: no-repeat;
}
.bio-all-content h6 {
  color: #fff;
}
.bio-all-content {
  position: relative;
  padding-bottom: 122px;
  padding-top: 78px;
}
.bio-all-content .img-bottom {
  position: absolute;
  width: 417px;
  bottom: -122px;
  right: 0;
}
.contact-us-wrap::before {
  content: "";
  background-image: url("../assets/images/Rocket.png");
  background-position: center;
  background-size: contain;
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  height: 295px;
  width: 250px;
  background-repeat: no-repeat;
}
.bio-all-content {
  position: relative;
}
.bio-all-content::before {
  content: "";
  position: absolute;
  left: 0;
  top: 134px;
  display: block;
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  background-image: url("../assets/images/bio-left.png");
  width: 210px;
  height: 364px;
}
.bio-all-content .img-bio-content {
  padding-bottom: 121px;
}
.two-col-biometric-wrap .bio-all-content p a {
  color: #fff;
}
@media only screen and (max-width: 1024px) {
  .two-col-biometric-wrap.bio-all-content {
    padding-top: 40px;
    padding-bottom: 9px;
  }
  .bio-all-content .img-bio-content {
    padding-bottom: 20px;
  }

  .bio-all-content .img-bottom {
    position: relative;
    width: 100%;
    bottom: -9px;
    right: 0;
    left: 0;
    text-align: center;
    margin: auto;
  }
}
@media only screen and (max-width: 993px) {
  .about-content-wrapper .img-about-content {
    margin-top: 0;
  }
}
</style>
