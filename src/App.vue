<template>
  <div id="app">
    <lpHeader/>
    <lp-main/>
    <lp-footer/>
  </div>
</template>

<script>
import lpHeader from './views/Header.vue'
import lpMain from './views/main.vue'
import lpFooter from './views/footer.vue'

export default {
  name: 'App',
  components: {
    lpHeader,
    lpMain,
    lpFooter
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
  --coffe: #aa897fa2;
  --grey: #e6e6e6;
  --red: #FD6F96;
  --redLg: #fd6f959f;
  --blue: #7fd4ff;
  --green: #71EFA3;
  --greenLg: #71efa39c;
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
