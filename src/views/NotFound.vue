<template>
  <div class="home">
    <AppHeader v-bind="props" />

    <div class="notfound-page">
      <div class="container">
        <div
          class="row d-flex justify-content-center align-items-center text-center"
        >
          <div class="col-12">
            <h2 class="blue-text">Page not found</h2>
            <img
              src="../assets/images/404-error.png"
              class="img-fluid"
              alt="404-error"
            />
            <h4>404: Resource not found</h4>
            <h5>This page does not exist. Sorry !!!</h5>
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
  name: "NotFound",
  components: { AppHeader, Footer },
  data: () => ({
    props: {
      tittle: "",
      content: ``,
      breadCrumb: {
        tittle: "",
        link: "/",
      },
    },
  }),
};
</script>
<style>
.notfound-page {
  padding: 70px 0;
}
.notfound-page img {
  margin-bottom: 20px;
}
</style>
