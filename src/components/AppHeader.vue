<script>
export default {
    data() {
        return {
            navItems: [
                {
                    text: "characters",
                    url: "#",
                    active: false,
                },
                {
                    text: "comics",
                    url: "#",
                    active: true,
                },
                {
                    text: "movies",
                    url: "#",
                    active: false,
                },
                {
                    text: "tv",
                    url: "#",
                    active: false,
                },
                {
                    text: "games",
                    url: "#",
                    active: false,
                },
                {
                    text: "collectibles",
                    url: "#",
                    active: false,
                },
                {
                    text: "videos",
                    url: "#",
                    active: false,
                },
                {
                    text: "fans",
                    url: "#",
                    active: false,
                },
                {
                    text: "news",
                    url: "#",
                    active: false,
                },
                {
                    text: "shop",
                    url: "#",
                    active: true,
                }
            ]
        }
    }
}
</script>

<template>
    <div class="header-container wrapper">
        <div class="img-container">
            <img src="../assets/dc-logo.png" alt="Dc logo">
        </div>
        <nav>
            <ul>
                <li v-for="navItem in navItems">{{ navItem.text }}</li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

div.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 125px;

    nav {
        height: 100%;

        ul {
            height: 100%;
            display: flex;
            align-items: center;

            li {
                color: $nav-main-color;
                text-transform: uppercase;
                height: 100%;
                font-weight: bolder;
                line-height: 118px;

                &:active,
                &:hover {
                    border-bottom: 6px solid $blue-banner;
                    color: $blue-banner;
                }
            }
        }
    }
}

img {
    padding: 10px;
}
</style>