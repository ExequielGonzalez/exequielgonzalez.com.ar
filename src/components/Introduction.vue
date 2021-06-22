<template>
  <section class="introduction grid absolute-top">
    <!-- <Background /> -->
    <p class="introduction__brief">
      Hola, yo soy
      <span class="introduction__brief-name">Exequiel Gonzalez</span>

      <typical
        class="typicalWrapper"
        :steps="['Web Developer', 1000, 'Estudiante de Ingeniería en Electrónica', 500, 'Y muchas otras cosas más! 👋', 1000]"
        :loop="Infinity"
        :wrapper="'h3'"
      ></typical>
    </p>
    <picture>
      <source
        class="introduction__photo"
        media="(min-width:600px)"
        srcset="../assets/foto3.png"
        alt="Foto de Exequiel Gonzalez"
      />

      <img class="introduction__photo" src="../assets/foto.png" alt="Foto de Exequiel Gonzalez" />
    </picture>
  </section>
</template>

<script>
import Background from "components/Background.vue";
import typical from "vue-typical";
export default {
  components: {
    typical
    // Background
  }
};
</script>

<style lang="scss" >
.typicalWrapper {
  padding-top: 10px;
  height: 200px;
  &::after {
    content: "|";
    animation: blink 1s infinite step-start;
  }
}
// picture {
//   position: relative;
// }
.introduction {
  //   scroll-snap-align: start;
  position: relative;
  align-items: center;
  // height: 0px;
  //   z-index: 1;
  @media (max-width: $s) {
    // height: 90vh;
    // position: relative;
  }
  &__brief {
    grid-column: 1/5;
    color: $accent;
    font-size: 4rem;
    line-height: 6rem;
    @media (max-width: $l) {
      grid-column: 1 / span 6;
      font-size: 3rem;
      line-height: 5rem;
    }
    @media (max-width: $m) {
      grid-column: 1 / span 3;
      font-size: 2.5rem;
      line-height: 4rem;
    }

    @media (max-width: $s) {
      position: absolute;
      top: 5%;
      grid-column: 1/-1;
      font-size: 1.8rem;
      line-height: 4rem;
    }

    &-name {
      display: block;
      color: $text-color;
      font-size: 10rem;
      line-height: 8rem;
      @media (max-width: $l) {
        grid-column: 1/2;
        font-size: 8rem;
        line-height: 6rem;
      }
      @media (max-width: $m) {
        grid-column: 1/2;
        font-size: 6rem;
        line-height: 4rem;
      }
      @media (max-width: $s) {
        grid-column: 1/-1;
        font-size: 4rem;
        line-height: 4rem;
      }
    }
  }
  &__photo {
    position: absolute;
    bottom: 0;
    grid-column: 6/12;
    // z-index: 1;
    width: 40vw;
    // @media (max-width: $l) {
    //   width: 650px;
    // }
    // @media (max-width: $m) {
    //   width: 500px;
    // }
    @media (max-width: $m) {
      width: 280px;
      width: 60vw;
      //   width: 50vw;
      // position: absolute;
      right: 0%;
      padding-left: -90px;
      // bottom: 50%;
      padding-bottom: -170px;
    }
    @media (max-width: $s) {
      width: 90vw;
      // max-height: 50%;
      // position: absolute;
      left: 00%;
      padding-left: -25px;
      bottom: 0;
      padding-bottom: 0;
    }
  }
}
</style>