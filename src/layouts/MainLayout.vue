<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar class="navbar grid">
        <h1 class="navbar__title">Exequiel Gonzalez</h1>

        <q-tabs
          class="navbar__tab"
          v-model="tab"
          indicator-color="transparent"
          active-color="accent"
          align="justify"
          :breakpoint="0"
        >
          <q-tab class="navbar__tab-init" name="tab1" label="Inicio" />
          <q-tab name="tab2" label="Acerca de mi" />
          <q-tab name="tab3" label="Experiencia" />
          <q-tab class="navbar__tab-contact" name="tab4" label="Contacto" />
        </q-tabs>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: "MainLayout",

  data() {
    return {
      tab: ""
    };
  }
};
</script>

<style lang="scss" scoped>
.navbar {
  margin-top: 20px;
  @media (max-width: $m) {
    margin-top: 0px;
  }
  &__title {
    grid-column: 1/5;
    font-size: 1.7rem;
    font-weight: 500;
    font-weight: 300;
    font-style: bold;
    line-height: 1.71rem;
    // font-family: "Roboto";

    @media (max-width: $m) {
      // grid-column: 0/0;
      display: none;
      // font-size: 1rem;
    }
  }
  &__tab {
    grid-column: 5/12;
    @media (max-width: $m) {
      margin-top: 0px;
      // display: inline-block;
      grid-column: 1/5;
      // display: none;
    }
    @media (max-width: $s) {
      // display: inline-block;
      // grid-column: 1/4;
      display: none;
    }
    // &-contact {
    //   color: $accent;
    //   border: 1px solid $accent;
    //   border-radius: 10px;
    // }
  }
}
</style>