<template>
  <header-section></header-section>
  <resume></resume>
</template>

<script>
import HeaderSection from "./components/HeaderSection.vue";
import Resume from "./components/Resume.vue";

export default {
  name: "App",
  components: {
    HeaderSection,
    Resume,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #212529;
  margin-top: 3rem;
}
</style>
