<script>
export default {
    name: "Cards",
    data() {
        return {
            cards: [
                {
                    img: 'h-2-port-img-1.jpg'
                },
                {
                    img: 'h-2-port-img-2.jpg'
                },
                {
                    img: 'h-2-port-img-3.jpg'
                },
                {
                    img: 'h-2-port-img-4.jpg'
                },
                {
                    img: 'h-2-port-img-5.jpg'
                },
                {
                    img: 'h-2-port-img-6.jpg'
                },
            ]
        }
    },
    methods: {
        getImagePath(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <section class="cards">
        <div v-for="element in cards" class="card_img">
            <img :src="getImagePath(element.img)" alt="">
        </div>
    </section>
</template>

<style scoped lang="scss">
.cards {
    display: flex;
    flex-wrap: wrap;
    width: 100%;
}

.card_img {
    width: calc(100% / 3);
    height: 100%;
}
</style>