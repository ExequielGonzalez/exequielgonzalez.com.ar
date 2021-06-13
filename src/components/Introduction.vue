<template>
  <section class="introduction grid">
    <p class="introduction__brief">
      Hola, yo soy
      <span class="introduction__brief-name">Exequiel Gonzalez</span>
      Web developer
    </p>
    <picture>
      <source
        class="introduction__photo"
        media="(min-width:600px)"
        srcset="../assets/foto2.png"
        alt="Foto de Exequiel Gonzalez"
      />

      <img class="introduction__photo" src="../assets/foto.png" alt="Foto de Exequiel Gonzalez" />
    </picture>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" >
.introduction {
  align-items: center;
  height: 100vh;
  //   z-index: 1;
  @media (max-width: $s) {
    height: 90vh;
  }
  &__brief {
    grid-column: 1/5;
    color: $accent;
    font-size: 4rem;
    line-height: 6rem;
    @media (max-width: $l) {
      grid-column: 1/6;
      font-size: 3rem;
      line-height: 5rem;
    }
    @media (max-width: $m) {
      grid-column: 1/3;
      font-size: 2.5rem;
      line-height: 4rem;
    }

    @media (max-width: $s) {
      grid-column: 1/4;
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
        grid-column: 1/4;
        font-size: 4rem;
        line-height: 4rem;
      }
    }
  }
  &__photo {
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
      //   width: 50vw;
      position: absolute;
      left: 60%;
      margin-left: -90px;
      bottom: 50%;
      margin-bottom: -170px;
    }
    @media (max-width: $s) {
      width: 210px;
      position: absolute;
      left: 50%;
      margin-left: -55px;
      bottom: 50%;
      margin-bottom: -140px;
    }
  }
}
</style>