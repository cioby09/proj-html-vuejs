<script>
export default {
    name: "Header",
    data() {
        return {
            menu: [
                {
                    title: "Home",
                    link: ""
                },
                {
                    title: "Pages",
                    link: ""
                },
                {
                    title: "Portfolio",
                    link: ""
                },
                {
                    title: "Blog",
                    link: ""
                },
                {
                    title: "Shop",
                    link: ""
                },
                {
                    title: "Elements",
                    link: ""
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/logo-sidearea-1.png" alt="Logo">
            </div>
            <nav class="nav-bar">
                <ul>
                    <li v-for="link in menu" :class="link.current ? 'active' : ''">
                        <a href="link.url">{{ link.title }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
$header-text: #464646;

header {
    height: 70px;
    width: 100%;
    padding: 0 1rem;
    background-color: white;

    .container {
        height: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .logo {
            margin: 0;

            img {
                height: 20px;
            }
        }

        .nav-bar {
            margin: 0;

            ul {
                display: flex;
                align-items: center;
                margin: 0;
                gap: 1rem;

                li {
                    list-style: none;

                    a {
                        text-decoration: none;
                        font-weight: 700;
                        font-size: 0.6rem;
                        text-transform: uppercase;
                        color: $header-text;
                    }
                }
            }
        }
    }
}
</style>
