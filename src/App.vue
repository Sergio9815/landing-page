<template>
  <div id="app">
    <lpHeader/>
    <lp-main/>
  </div>
</template>

<script>
import lpHeader from './components/lpHeader.vue'
import lpMain from './components/lpMain.vue'

export default {
  name: 'App',
  components: {
    lpHeader,
    lpMain
  }
}
</script>

<style>

html {
  scroll-behavior: smooth;
}

/* --- --- -- COLORS -- --- --- */
:root {
  --dark: #161616;
  --darkLg: #1616163b;
  --white: #ffff;
  --brown: #7D5A50;
  --brownLg: #7d5a50a8;
  --grey: #e6e6e6;
  --red: #FD6F96;
  --blue: #7fd4ff;
  --green: #71EFA3;
}

body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
