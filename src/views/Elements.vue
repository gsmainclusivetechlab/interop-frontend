<template>
  <div class="home">
    <AppHeader v-bind="props" />
  </div>
</template>

<script>
import AppHeader from "../components/AppHeader";
export default {
  name: "Elements",
  components: { AppHeader },
  data: () => ({
    props: {
      tittle: "These are the features B4LL brings to you",
      content: `See how the features of our showcase can help mobile operators to bring the power of biometrics`,
      breadCrumb: {
        tittle: "How it works",
        link: "/howitworks",
      },
    },
  }),
};
</script>