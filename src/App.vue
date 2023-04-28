<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue"

export default {
  components: {
    Header,
    Jumbotron
  }
}
</script>

<template>
  <Header />
  <Jumbotron />
</template>

<style lang="scss">
@use "./style/general.scss" as *;
</style>
