<script>
import Jumbotron from "./Jumbotron.vue";
import Cards from "./Cards.vue";
import Section1 from "./Section1.vue";
import Section2 from "./Section2.vue";
import Section3 from "./Section3.vue";

export default {
    name: "Main",
    components: {
        Jumbotron,
        Cards,
        Section1,
        Section2,
        Section3
    }
}
</script>

<template>
    <Jumbotron />
    <Cards />
    <Section1 />
    <Section2 />
    <Section3 />
</template>

<style></style>