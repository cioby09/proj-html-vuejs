<script>
export default {
    name: "Section1",
    data() {
        return {
            process: [
                {
                    logo: "fa-solid fa-lightbulb",
                    title: "First theres an idea",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, optio in. Modi, repellendus exercitationem!"
                },
                {
                    logo: "fa-regular fa-comment",
                    title: "Then we talk about",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, optio in. Modi, repellendus exercitationem!"
                },
                {
                    logo: "fa-solid fa-cloud",
                    title: "And we think about",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, optio in. Modi, repellendus exercitationem!"
                },
                {
                    logo: "fa-solid fa-pencil",
                    title: "So we draw along",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, optio in. Modi, repellendus exercitationem!"
                },
            ]
        }
    }
}
</script>

<template>
    <section class="section1">
        <div class="container">
            <h2>Working process</h2>

            <div class="process">
                <div v-for="element in process" class="process-card">
                    <i class="element.logo"></i>
                    <h3 class="title">{{ element.title }}</h3>
                    <p class="text">{{ element.text }}</p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.section1 {
    width: 100%;
    height: 400px;
    margin: 0 auto;

    .container {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        max-width: 1000px;
        text-align: center;

        .process {
            height: 150px;
            display: flex;
            background-color: white;
            width: 800px;

            .process-card {
                width: calc(100% / 4);

                h3 {
                    font-size: 1rem;
                }

                .text {
                    font-size: 0.7rem;
                }
            }
        }
    }
}
</style>