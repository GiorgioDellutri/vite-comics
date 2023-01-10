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

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

div.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    nav ul {
        display: flex;
        align-items: center;

        li {
            color: $nav-main-color;
            text-transform: uppercase;

            &:active,
            &:hover {
                color: $blue-banner;
            }
        }
    }
}

img {
    padding: 10px;
}
</style>