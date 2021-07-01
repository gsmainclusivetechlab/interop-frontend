<template>
  <div class="topbar">
    <header>
      <b-container fluid>
        <b-navbar toggleable="lg">
          <b-navbar-brand href="/">
            <img
              src="../../assets/images/Logol1img.jpg"
              class="img-fluid normal-logo "
              alt="Logo"
          /></b-navbar-brand>

          <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

          <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav class="ml-auto">
              <b-navbar-nav>
                <b-nav-item href="#">
                  <router-link to="/">Home</router-link>
                </b-nav-item>
                <b-nav-item href="#">
                  <router-link to="/howitworks">How it works</router-link>
                </b-nav-item>
                <b-nav-item href="#">
                  <router-link to="/tryb4all"> Try B4LL </router-link>
                </b-nav-item>
                <b-nav-item href="https://docs.biometrics.gsmainclusivetechlab.io/">
                  <!-- <router-link to="/documentation">  -->
                  <a href=" https://docs.biometrics.gsmainclusivetechlab.io/ "
                    >Documentation</a
                  >
                  <!-- </router-link> -->
                </b-nav-item>
                <b-nav-item href="#">
                  <router-link to="/about">About</router-link>
                </b-nav-item>
                <b-nav-item href="#">
                  <router-link to="/faq">FAQs</router-link>
                </b-nav-item>
              </b-navbar-nav>
            </b-navbar-nav>
          </b-collapse>
        </b-navbar>
        <ul class="lang-menu">
          <li class="init">
            <!-- <a href="#">
            <img
              src="../../assets/images/globe-icon.svg"
              class="img-fluid"
              alt="globe-icon"
            />
            </a> -->
          </li>
        </ul>
      </b-container>
    </header>
  </div>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style>
.dropdown-down-logo {
  margin-left: -30px;
}
.navbar {
  background-color: transparent !important;
  padding: 20px 0;
  letter-spacing: 1px;
  background: 0 0;
  padding-right: 80px;
}
.topbar .navbar-light .navbar-nav .nav-link a,
.topbar .navbar-light .navbar-nav .nav-item.dropdown .nav-link a,
.navbar-light .navbar-nav .nav-item.dropdown .nav-link.dropdown-toggle {
  color: #fff !important;
  font-size: 16px;
  padding: 10px 20px;
  line-height: normal;
  font-weight: 400;
}

.navbar-brand .normal-logo {
  width: 66px;
  height: 64px;
}
.navbar-light .navbar-nav li a {
  color: #fff !important;
  font-size: 16px;
  font-weight: 400;
}
.topbar .navbar-nav .show > .nav-link {
  color: #fdfdfe !important;
}
.topbar .navbar-light .navbar-nav .nav-link:focus,
.topbar .navbar-light .navbar-nav .nav-link:hover {
  color: white !important;
}
.navbar-light .navbar-nav .active > .nav-link,
.navbar-light .navbar-nav .nav-link.active,
.navbar-light .navbar-nav .nav-link.show,
.navbar-light .navbar-nav .show > .nav-link {
  color: white !important;
}

.lang-menu {
  height: 27px;
  padding-right: 42px;
  position: absolute;
  padding-left: 0;
  right: 35px;
  top: 40px;
}
ul.search-bar {
  padding: 0;
  padding-left: 0;
  position: absolute;
  right: 20px;
  top: 45px;
}
a:hover {
  /* color: #ffffff; */
  text-decoration: none;
}
a {
  font-weight: 400;
  font-size: 16px;
  color: #000;
}
.navbar .dropdown-toggle:after {
  content: "";
  background-image: url("../../assets/images/arrow-white.svg");
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  font-size: 18px;
  position: absolute;
  border: none;
  bottom: 16px;
  right: 0;
  width: 10px;
  height: 10px;
  line-height: 10px;
}
.navbar-light .navbar-nav .nav-item {
  display: flex;
  justify-content: center;
  align-items: center;
}
.navbar-light .navbar-nav li a {
  padding: 10px 20px;
}
.navbar-light .navbar-nav .dropdown-item:hover,
.navbar-light .navbar-nav .dropdown-item.active {
  color: #6b3076 !important;
  background: #fff;
  border-radius: 10px;
}
.navbar-expand-lg .navbar-nav .dropdown-menu {
  background: #fff;
  padding: 0;
  margin: 0;

  box-shadow: 0 16px 40px rgb(0 0 0 / 10%);
  /* border-radius: 10px;
    
    padding-top: 34px;
    padding-left: 24px;
    padding-right: 24px;
    min-width: 271px;
    min-height: 201px;
  
    padding-bottom: 28px;
        top: 45px; */
}
.nav-link:focus,
.nav-link:hover {
  border: none;
  outline: none;
}

.navbar-light .navbar-toggler-icon {
  background-image: url("../../assets/images/menu.png");
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
}
.navbar-light .navbar-toggler {
  color: transparent;
  border-color: transparent;
}
.navbar-expand-lg .navbar-nav .dropdown-menu li a {
  color: #373737 !important;
}
@media only screen and (min-width: 1025px) {
  .navbar {
    padding-left: 29px;
    margin-right: 0;
    padding-right: 55px;
  }
  .lang-menu {
    right: 0px;
  }
  ul.search-bar {
    right: 55px;
  }
}
@media only screen and (min-width: 1024px) {
  .navbar-light .navbar-nav .nav-item .nav-link a.router-link-exact-active {
    position: relative;
  }
  .navbar-expand-lg .navbar-nav .dropdown-menu::after {
    content: "";
    width: 0;
    height: 0;
    border-left: 9px solid transparent;
    border-right: 9px solid transparent;
    border-bottom: 9px solid #fff;
    position: absolute;
    right: 22px;
    top: -9px;
  }
  .navbar-light
    .navbar-nav
    .nav-item
    .nav-link
    a.router-link-exact-active::after {
    content: "";
    width: 100%;
    height: 2px;
    background-color: #ae52c4;
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
  }
  .navbar-expand-lg .navbar-nav .dropdown-menu {
    background: #fff;
    padding: 0;
    margin: 0;
    right: -28px;

    box-shadow: 0 16px 40px rgb(0 0 0 / 10%);
    border-radius: 10px;

    padding-top: 34px;
    padding-left: 24px;
    padding-right: 24px;
    /* min-width: 271px; */
    /* min-height: 201px; */
    /* bottom: -27px; */
    padding-bottom: 28px;
    top: 45px;
  }
}
@media only screen and (max-width: 993px) {
  .navbar-light .navbar-nav .nav-item .nav-link a.router-link-exact-active {
    font-weight: 700;
  }
  .navbar-light .navbar-nav .nav-item {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    /* padding-left: 0; */
    flex-direction: column;
    border-bottom: 1px solid #fff;
  }

  .topbar .navbar-light .navbar-nav .nav-link a,
  .topbar .navbar-light .navbar-nav .nav-item.dropdown .nav-link a,
  .navbar-light .navbar-nav .nav-item.dropdown .nav-link.dropdown-toggle {
    padding-left: 19px;
  }
  .navbar-expand-lg .navbar-nav .dropdown-menu li a {
    padding-left: 19px;
  }
  .navbar-light .navbar-nav li a {
    padding-left: 0;
  }
  .navbar-nav {
    background: #95236c;
  }

  .dropdown-down-logo {
    margin-left: 0;
    width: 20px;
    height: 20px;
  }
  .navbar-expand-lg .navbar-nav .dropdown-menu {
    position: relative;
    padding-left: 0;
    width: 100%;
    border-radius: none;
  }
  .navbar-nav {
    background: #95236c;
  }
  .navbar {
    padding-right: 0;
  }
  .lang-menu {
    right: 40px;
  }
  ul.search-bar {
    right: 85px;
  }
  .navbar .dropdown-toggle:after {
    right: 23px;
    top: 16px;
    bottom: 0;
  }
}
</style>
