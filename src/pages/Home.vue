<template>
  <q-page>
    <Background style="opacity:1" />
    <div class="landing">
      <Introduction class="landing__introduction" />
      <!-- <div>asd</div> -->
      <!-- <Introduction class="landing__introduction" /> -->
      <!-- <Introduction class="landing__introduction" /> -->

      <!-- <q-btn class="test" color="primary" icon="check" label="OK" /> -->
      <!-- <q-btn class="test2" color="primary" icon="check" label="OK" /> -->
      <ContactForm />
      <Contact />
    </div>
  </q-page>
</template>

<script>
import Introduction from "components/Introduction.vue";
import ContactForm from "components/ContactForm.vue";
import Contact from "components/Contact.vue";
import Background from "components/Background.vue";
export default {
  name: "PageHome",
  components: { Introduction, Background, Contact, ContactForm }
  // components: { Introduction, Contact, ContactForm }
};
</script>

<style lang="scss" >
// .test {
//   grid-column: 1/-1;
// }

// .test2 {
//   grid-column: 1/3;
// }
.landing {
  scroll-snap-type: mandatory;
  scroll-snap-points-y: repeat(3rem);
  scroll-snap-type: y mandatory;
  // overflow-y: scroll;
  &__introduction {
    height: calc(100vh - 68px);
    // height: 100vh;
    scroll-snap-align: start;
  }
}
</style>