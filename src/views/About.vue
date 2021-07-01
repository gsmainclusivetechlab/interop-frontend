<template>
  <div class="home">
    <AppHeader v-bind="props" />
    <div class="about-content-wrapper">
      <div class="container">
        <div class="row">
          <div class="col-12 col-md-6">
            <h2>Inclusive Tech Lab</h2>
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
          <div class="col-12 col-md-6">
            <div class="img-about-content">
              <img
                src="../assets/images/Tech-lab.png"
                class="img-fluid"
                alt="Tech-lab"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <section class="two-col-biometric-wrap text-white bio-all-content">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <div class="bio-all-content-wrap">
              <h2>Biometrics for All</h2>
            </div>
          </div>
          <div class="col-12 col-lg-6">
            <div class="bio-all-content-wrap">
              <h6>
                Biometrics for All seeks to show digital service providers the advantages and possibilities of using biometric solutions in low-tech environments. The main advantage of using biometrics in low tech environments comes from the ability to reach a larger audience of users.
              </h6>
              <h6>
                This benefit is even more evident in places where the number of
                national ID holders is reduced. Thus, in some developing
                countries, starting from a scenario where access to national ID
                is difficult, the registration and authentication of users on
                mobile operators may be compromised. In this sense, the use of
                biometrics allows the use of non-transferable information,
                leading to greater adherence by users. This makes biometrics the
                ideal and more accurate solution for validating personal data.
              </h6>
              
            </div>
          </div>
          <div class="col-12 col-lg-6">
            <div class="img-bio-content">
              <h6>
                If well implemented, biometrics authentication can unlock access
                to a large number of previously difficult to reach customers,
                such as: people with disabilities, less literate populations,
                people with lack of national ID, featured phones users and much more.
              </h6>
              <h6>
                The use of biometrics can increase the security to execute
                mobile money transactions, such as international remittance.
                Inscribed within well-designed platforms would not only enable
                them to make greater and better use of their mobile wallets, but
                also make usage more secure and attractive.
              </h6>
              <h6>
                The GSMA is working with its members and mobile money industry
                partners to support the process of implementing biometrics in
                their markets.
              </h6>
            </div>
            <div class="img-bottom">
              <img
                src="../assets/images/Biomet.png"
                class="img-fluid"
                alt="Biomet"
              />
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
  background-image: url("../assets/images/dotr.png");
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
