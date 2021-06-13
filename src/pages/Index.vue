<template>
  <q-page>
    <Background />
    <div>
      <Introduction />
      <!-- <Introduction /> -->

      <!-- <q-btn class="test" color="primary" icon="check" label="OK" /> -->
      <!-- <q-btn class="test2" color="primary" icon="check" label="OK" /> -->
    </div>
  </q-page>
</template>

<script>
import Introduction from "components/Introduction.vue";
import Background from "components/Background.vue";
export default {
  name: "PageIndex",
  components: { Introduction, Background }
};
</script>

<style lang="scss" >
// .test {
//   grid-column: 1/-1;
// }

// .test2 {
//   grid-column: 1/3;
// }
</style>