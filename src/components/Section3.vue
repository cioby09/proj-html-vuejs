<script>
export default {
    name: "Section3",
    data() {
        return {
            events: [
                {
                    img: 'h-2-blog-img-1.jpg',
                    title: 'This way, loves: a detailed guide through new design',
                    author: 'By Emily Fields'
                },
                {
                    img: 'h-2-blog-img-2.jpg',
                    title: 'I try to give people a different way of looking art',
                    author: 'By Emily Fields'
                },
                {
                    img: 'h-2-blog-img-3.jpg',
                    title: 'Introduce Richard Laperrière of those amazing features',
                    author: 'By Emily Fields'
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
    <section class="section3">
        <div class="container">
            <div v-for="element in events" class="event-card">
                <img :src="getImagePath(element.img)" alt="">
                <h3>{{ element.title }}</h3>
                <p>{{ element.author }}</p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.section3 {
    width: 100%;
    height: 400px;
    background-color: white;

    .container {
        max-width: 800px;
        height: 100%;
        display: flex;
        align-items: center;
        gap: 2rem;

        .event-card {
            width: calc(100% / 3);

            h3 {
                font-size: 1rem;
            }
        }
    }
}
</style>