<template>
  <div id="app" class="app">
    <router-view />
    <Footer />
    <notifications />
  </div>
</template>

<script>
export default {
  name: "app",
};
</script>
<style>
@font-face {
  font-family: "Arial";
  font-style: normal;
  font-weight: normal;
  src: url("./fonts/arialregular.eot"); /* IE9 Compat Modes */
  src: url("./fonts/arialregular.eot?#iefix") format("embedded-opentype"),
    /* IE6-IE8 */ url("./fonts/arialregular.woff") format("woff"),
    /* Modern Browsers */ url("./fonts/arialregular.ttf") format("truetype"),
    /* Safari, Android, iOS */ url("./fonts/arialregular.svg#Arial")
      format("svg"); /* Legacy iOS */
}

@font-face {
  font-family: "Arial";
  font-style: normal;
  font-weight: bold;
  src: url("./fonts/arialbold.eot"); /* IE9 Compat Modes */
  src: url("./fonts/arialbold.eot?#iefix") format("embedded-opentype"),
    /* IE6-IE8 */ url("./fonts/arialbold.woff") format("woff"),
    /* Modern Browsers */ url("./fonts/arialbold.ttf") format("truetype"),
    /* Safari, Android, iOS */ url("./fonts/arialbold.svg#Arial") format("svg"); /* Legacy iOS */
}

body,
html {
  overflow: hidden;
  overflow-y: auto;
  color: #000000;
}
a {
  font-weight: bold;
  /* color: #fff; */
}
.app {
  font-family: "Arial";
  font-size: 16px;
  line-height: normal;
  line-height: 26px;
  font-weight: 400;
}
a,
a:hover {
  text-decoration: none;
  /* color:#ae52c4; */
}
a:hover,
p a:hover,
p a {
  color: #ae52c4;
}
h1 {
  font-size: 42px;
  font-weight: bold;
  color: #ffffff;
}
h2 {
  font-size: 30px;
  font-weight: bold;
  line-height: 43px;
  padding-bottom: 18px;
}
h3 {
  font-size: 28px;
  font-weight: bold;
  color: #373737;
  padding-bottom: 18px;
  margin-bottom: 0;
}
h4 {
  font-size: 18px;
  font-weight: 600;
  color: #373737;
  line-height: 30px;
}
h5 {
  font-size: 17px;
  font-weight: bold;
  line-height: 30px;
}
h6 {
  font-size: 16px;
  line-height: 26px;
  color: #373737;
}
p {
  font-weight: 400;
  font-size: 16px;
  letter-spacing: normal;
  padding-bottom: 10px;
  line-height: 26px;
}
.bg-greys {
  background-color: #fafbfe;
}
.blue-text {
  color: #95236c;
}
@media only screen and (max-width: 993px) {
  h1 {
    font-size: 27px;
  }
}
</style>
