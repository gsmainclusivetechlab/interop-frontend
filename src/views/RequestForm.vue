<template>
  <div class="home-form">
    <AppHeader v-bind="props" />
    <iframe title="form" :src="source" width="100%" height="100%"></iframe>
  </div>
</template>

<script>
import AppHeader from "../components/AppHeader";

export default {
  name: "RequestForm",
  components: { AppHeader },

  data: () => ({
    props: {
      tittle: "Request Form",
      breadCrumb: {
        tittle: "Request Form",
        link: "requestform",
      },
    },
    source: "./requestForm.html",
  }),
};
</script>

<style>
.home-form iframe {
  height: 130vh;

  width: 100vw;

  border: none;
  border: none;
}

.home-form .topbar {
  background: #95236c;
}
</style>
