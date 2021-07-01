<template>
  <div class="inner-header">
    <NavBar />
    <div
      v-bind:class="[
        breadCrumb.link === 'tryb4all'
          ? 'inner-head-try'
          : breadCrumb.link === 'about'
          ? 'inner-head-about'
          : 'inner-header-wrap',
      ]"
    >
      <div class="inner-banner-wrapper">
        <div class="container">
          <div class=" row">
            <div class="col-12">
              <div class="inner-content-frame">
                <h3>{{ tittle }}</h3>
                <h4>
                  {{ content }}
                </h4>
              </div>
              <div class="pagination-content">
                <ul>
                  <li><a href="/">Home</a></li>
                  <li>
                    {{ breadCrumb.tittle }}
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavBar from "./layout/NavBar";
export default {
  name: "AppHeader",
  components: { NavBar },
  props: {
    tittle: String,
    content: String,
    breadCrumb: {
      tittle: String,
      link: String,
    },
  },
};
</script>

<style>
.inner-header .topbar header {
  padding: 0;
  position: absolute;
  z-index: 999;
  width: 100%;
  -webkit-transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
  transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
  min-height: 100px;
  transition: all 0.5s ease-out;
  background: transparent;
}
.inner-header .inner-header-wrap,
.inner-header .inner-head-try,
.inner-header .inner-head-about {
  width: 100%;
  color: #fff;
  padding: 132px 0 29px;
  background-color: #aaa;
  background-repeat: no-repeat !important;
  background-position: center center !important;
  background-size: cover !important;
  position: relative;
  z-index: 0;
}
.inner-header .inner-header-wrap::before,
.inner-header .inner-head-try::before {
  content: "";
  background-image: url("../assets/images/inner-dot-bg.png");
  background-position: top;
  position: absolute;
  top: 0;
  left: 0;
  width: 226px;
  height: 235px;
  background-repeat: no-repeat;
}
.inner-header .inner-header-wrap {
  background-image: url("../assets/images/security.png");
  background-position: center;
  background-repeat: no-repeat;
  min-height: 374px;
  width: 100%;
  color: #fff;
}
.inner-header .inner-head-try {
  background-image: url("../assets/images/bg-try.png");
  background-position: center;
  background-repeat: no-repeat;
  min-height: 374px;
  width: 100%;
  color: #fff;
}
.inner-header .inner-head-about {
  background-image: url("../assets/images/banner.png");
  background-position: center;
  background-repeat: no-repeat;
  min-height: 374px;
  width: 100%;
  color: #fff;
}
.inner-banner-wrapper h3,
.inner-banner-wrapper h4 {
  color: #fff;
}
.inner-content-frame {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  flex-direction: column;
  padding-bottom: 40px;
  white-space: normal;
}
.inner-header .inner-banner-wrapper {
  min-height: 213px;
  display: flex;
  justify-content: flex-start;
  align-items: flex-end;
  position: relative;
}
.pagination-content ul {
  padding-left: 0;
  display: block;
  margin-bottom: 0;
}
.pagination-content ul li,
.pagination-content ul li a {
  font-size: 13px;
  color: #fff;
}
.pagination-content ul li a:hover {
  color: #fff;
}
.pagination-content ul li {
  display: inline-block;
  padding-right: 25px;
  position: relative;
  font-size: 13px;
}
.pagination-content ul li::after {
  content: "/";

  position: absolute;
  right: 9px;
  top: 0;
  bottom: 0;
}
.pagination-content ul li:last-child:after {
  content: " ";
  display: none;
}
.pagination-content ul li:last-child a {
  font-weight: bold;
}

@media only screen and (max-width: 993px) {
  .inner-header .topbar header {
    padding: 0;
    position: absolute;
    z-index: 999;
    width: 100%;
    -webkit-transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
    transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
    min-height: 100px;
    transition: all 0.5s ease-out;
    background: transparent;
  }
  .inner-header .inner-header-wrap {
    width: 100%;
    color: #fff;
    padding: 132px 0 29px;
    background-color: #aaa;
    background-repeat: no-repeat !important;
    background-position: center center !important;
    background-size: cover !important;
    position: relative;
    z-index: 0;
  }
}
</style>
