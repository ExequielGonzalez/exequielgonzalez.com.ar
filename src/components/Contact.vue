<template>
  <section class="contact subgrid">
    <h3 class="contact__title">Exequiel Gonzalez</h3>
    <p class="contact__quote">"Ningún soñador es pequeño y ningún sueño es demasiado grande"</p>

    <div class="contact__info">
      <p class="contact__info-label">
        <q-icon size="20px" color="accent" name="location_on" />Paraná, Entre Rios, Argentina
      </p>
      <p class="contact__info-label">
        <q-icon size="20px" color="accent" name="email" />contacto@exequielgonzalez.com.ar
      </p>
      <p class="contact__info-label">
        <q-icon size="20px" color="accent" name="phone_in_talk" />+54 0343-155131659
      </p>
    </div>
    <div class="contact__pages">
      <q-icon
        class="contact__icon"
        tag="a"
        href="https://www.linkedin.com/in/exequielgonzalez/"
        target="_blank"
        name="fab fa-linkedin"
        size="40px"
        color="white"
      />
      <q-icon
        class="contact__icon"
        tag="a"
        href="https://github.com/ExequielGonzalez"
        target="_blank"
        name="fab fa-github-square"
        size="40px"
        color="white"
      />
    </div>
    <p></p>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
.contact {
  height: 100vh;
  width: 100%;
  background-color: $footer;
  background: #141e30; /* fallback for old browsers */
  background: -webkit-linear-gradient(
    to top,
    #243b55,
    #141e30
  ); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(
    to top,
    #243b55,
    #141e30
  ); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  @media (min-width: $m) {
    height: 40vh;
  }
  &__title {
    grid-column: 1/-1;
    padding-top: 50px;
    font-size: 3.5rem;
    letter-spacing: 1px;
    text-align: center;
    color: $accent;
  }
  &__quote {
    grid-column: 1/-1;
    text-align: center;
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
    font-style: italic;
    color: $accent-light;
  }
  // &__info-small {
  //   grid-column: 2 / span3;
  //   display: flex;
  //   @media (min-width: $m) {
  //     display: none;
  //   }
  //   &-label {
  //     padding-left: 5px;
  //   }
  // }
  &__info {
    grid-column: 1/-1;
    display: flex;
    flex-direction: column;
    align-content: stretch;
    justify-content: space-evenly;
    align-items: flex-start;
    @media (min-width: $m) {
      flex-direction: row;
    }
    &-label {
      place-items: center;
      align-items: center;
      align-content: center;
      align-self: center;
      // padding-left: 20px;
    }
  }
  &__pages {
    grid-column: 1 / -1;
    display: flex;
    // align-items: center;
    justify-content: center;
  }
  &__icon {
    width: 100px;
  }
}
</style>