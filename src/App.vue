<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import Cards from "./components/Cards.vue";

export default {
  components: {
    Header,
    Jumbotron,
    Cards
  }
}
</script>

<template>
  <Header />
  <Jumbotron />
  <Cards />
</template>

<style lang="scss">
@use "./style/general.scss" as *;
</style>
