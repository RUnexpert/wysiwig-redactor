<template>
  <main class="container">
    <the-editor></the-editor>
  </main>
</template>

<script>
import TheEditor from "./components/TheEditor.vue";

export default {
  name: "App",
  components: {
    TheEditor,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap");

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  box-sizing: inherit;
}

#app {
  margin-top: 40px;
  margin-bottom: 40px;
}

body {
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-style: normal;
  font-size: 16px;
  line-height: 23px;
  letter-spacing: 0.6px;
  background-color: #1e1e1e;
  color: #ffffff;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
