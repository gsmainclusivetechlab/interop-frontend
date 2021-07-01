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
                <b-nav-item
                  href="https://docs.biometrics.gsmainclusivetechlab.io/"
                >
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
            <!-- <a href="#"> -->
            <img
              src="../../assets/images/globe-icon.svg"
              class="img-fluid"
              alt="globe-icon"
            />
            <!-- </a> -->
          </li>
        </ul>
      </b-container>
    </header>
  </div>
</template>

<script>
export default {
  name: "RequestFormNav",
};
</script>

<style>
.home-form .dropdown-down-logo {
  margin-left: -30px;
}
.home-form .navbar {
  background-color: purple;
  padding: 20px 0;
  letter-spacing: 1px;
  background: 0 0;
  padding-right: 80px;
}
.home-form .topbar .navbar-light .navbar-nav .nav-link a,
.home-form .topbar .navbar-light .navbar-nav .nav-item.dropdown .nav-link a,
.home-form
  .navbar-light
  .navbar-nav
  .nav-item.dropdown
  .nav-link.dropdown-toggle {
  /* color: rgb(13, 10, 36) !important; */
  font-size: 16px;
  padding: 10px 20px;
  line-height: normal;
  font-weight: 400;
}

.home-form .navbar-brand .normal-logo {
  width: 66px;
  height: 64px;
}
.home-form .navbar-light .navbar-nav li a {
  color: rgb(24, 7, 37) !important;
  font-size: 16px;
  font-weight: 400;
}
.home-form .topbar .navbar-nav .show > .nav-link {
  color: #1f032c !important;
}
.home-form .topbar .navbar-light .navbar-nav .nav-link:focus,
.home-form .topbar .navbar-light .navbar-nav .nav-link:hover {
  color: rgb(23, 6, 39) !important;
}
.home-form .navbar-light .navbar-nav .active > .nav-link,
.home-form .navbar-light .navbar-nav .nav-link.active,
.home-form .navbar-light .navbar-nav .nav-link.show,
.home-form .navbar-light .navbar-nav .show > .nav-link {
  color: rgb(21, 8, 32) !important;
}

.home-form .lang-menu {
  height: 27px;
  padding-right: 42px;
  position: absolute;
  padding-left: 0;
  right: 35px;
  top: 40px;
}
.home-form ul.search-bar {
  padding: 0;
  padding-left: 0;
  position: absolute;
  right: 20px;
  top: 45px;
}
.home-form a:hover {
  /* color: #ffffff; */
  text-decoration: none;
}
.home-form a {
  font-weight: 400;
  font-size: 16px;
  color: #000;
}
.home-form .navbar .dropdown-toggle:after {
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
.home-form .navbar-light .navbar-nav .nav-item {
  display: flex;
  justify-content: center;
  align-items: center;
}
/* .home-form .navbar-light .navbar-nav li a {
  padding: 10px 20px;
} */
.home-form .navbar-light .navbar-nav .dropdown-item:hover,
.home-form .navbar-light .navbar-nav .dropdown-item.active {
  color: #6b3076 !important;
  background: #fff;
  border-radius: 10px;
}
.home-form .navbar-expand-lg .navbar-nav .dropdown-menu {
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
.home-form .nav-link:focus,
.home-form .nav-link:hover {
  border: none;
  outline: none;
}

.home-form .navbar-light .navbar-toggler-icon {
  background-image: url("../../assets/images/menu.png");
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
}
.home-form .navbar-light .navbar-toggler {
  color: transparent;
  border-color: transparent;
}
.home-form .navbar-expand-lg .navbar-nav .dropdown-menu li a {
  color: #373737 !important;
}
@media only screen and (min-width: 1025px) {
  .home-form .navbar {
    padding-left: 29px;
    margin-right: 0;
    padding-right: 55px;
  }
  .home-form .lang-menu {
    right: 0px;
  }
  .home-form ul.search-bar {
    right: 55px;
  }
}
@media only screen and (min-width: 1024px) {
  .home-form
    .navbar-light
    .navbar-nav
    .nav-item
    .nav-link
    a.router-link-exact-active {
    position: relative;
  }
  .home-form .navbar-expand-lg .navbar-nav .dropdown-menu::after {
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
  .home-form
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
  .home-form .navbar-expand-lg .navbar-nav .dropdown-menu {
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
  .home-form
    .navbar-light
    .navbar-nav
    .nav-item
    .nav-link
    a.router-link-exact-active {
    font-weight: 700;
  }
  .home-form .navbar-light .navbar-nav .nav-item {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    /* padding-left: 0; */
    flex-direction: column;
    border-bottom: 1px solid #fff;
  }

  .home-form .topbar .navbar-light .navbar-nav .nav-link a,
  .home-form .topbar .navbar-light .navbar-nav .nav-item.dropdown .nav-link a,
  .home-form
    .navbar-light
    .navbar-nav
    .nav-item.dropdown
    .nav-link.dropdown-toggle {
    padding-left: 19px;
  }
  .home-form .navbar-expand-lg .navbar-nav .dropdown-menu li a {
    padding-left: 19px;
  }
  .home-form .navbar-light .navbar-nav li a {
    padding-left: 0;
  }
  .home-form .navbar-nav {
    background: #95236c;
  }

  .home-form .dropdown-down-logo {
    margin-left: 0;
    width: 20px;
    height: 20px;
  }
  .home-form .navbar-expand-lg .navbar-nav .dropdown-menu {
    position: relative;
    padding-left: 0;
    width: 100%;
    border-radius: none;
  }
  .home-form .navbar-nav {
    background: #95236c;
  }
  .home-form .navbar {
    padding-right: 0;
  }
  .home-form .lang-menu {
    right: 40px;
  }
  .home-form ul.search-bar {
    right: 85px;
  }
  .home-form .navbar .dropdown-toggle:after {
    right: 23px;
    top: 16px;
    bottom: 0;
  }
}
</style>
