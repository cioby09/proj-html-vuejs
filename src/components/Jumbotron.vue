<script>
export default {
    name: "Jumbotron",
    data() {
        return {

        }
    }
}
</script>

<template>
    <section class="jumbotron">
        <div class="container">
            <div class="info">
                <h1>Devotion that never ends</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium tenetur corrupti similique quaerat
                    sapiente distinctio consequuntur porro, sint nostrum sit at eum sunt numquam in maxime aut et
                    perferendis ad.</p>
                <div class="btn btn-primary">Read more</div>
            </div>
            <div class="image">
                <img src="../assets/img/h-2-slider-img-11.png" alt="">
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.jumbotron {
    height: 350px;
    width: 100%;
    background-color: white;

    .container {
        max-width: 1000px;
        height: 100%;
        display: flex;
        align-items: center;

        .info {
            width: 40%;
        }

        .image {
            width: 60%;
        }
    }
}
</style>