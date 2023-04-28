<script>
import Jumbotron from "./Jumbotron.vue";
import Cards from "./Cards.vue";
import Section1 from "./Section1.vue";

export default {
    name: "Main",
    components: {
        Jumbotron,
        Cards,
        Section1
    }
}
</script>

<template>
    <Jumbotron />
    <Cards />
    <Section1 />
</template>

<style></style>