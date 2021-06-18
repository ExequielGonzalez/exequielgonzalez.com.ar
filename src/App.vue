<template>
  <div id="q-app">
    <router-view />
  </div>
</template>
<script>
export default {
  name: "App"
};
</script>

<style lang="scss">
body.body--dark {
  background: $background;
}

html {
  background-image: url("./assets/foto3.png"), url("./assets/foto.png");

  background-size: 0;
}
</style>