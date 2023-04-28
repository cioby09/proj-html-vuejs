<script>
export default {
    name: "Footer"
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="footer-card">
                <img src="../assets/img/logo-sidearea-1.png" alt="Logo">
                <p>Let's Get creative</p>
            </div>
            <div class="footer-card">
                <p>maree.qode@gmail.com</p>
                <p>+44645 321 789</p>
            </div>
            <div class="footer-card">
                <p>Avenue d'Auderghem 10</p>
                <p>1040 Brussels, Belgium</p>
            </div>
            <div class="footer-card">
                <p>Stay in touch with us</p>
                <div class="social">
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-pinterest-p"></i>
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-linkedin-in"></i>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
footer {
    width: 100%;
    height: 200px;
    background-color: #DBF0E3;

    .container {
        max-width: 800px;
        height: 100%;
        display: flex;
        align-items: center;
    }
}
</style>