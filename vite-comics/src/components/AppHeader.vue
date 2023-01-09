<template>
    <div class="header-container wrapper">
        <div class="img-container">
            <img src="../assets/dc-logo.png" alt="Dc logo">
        </div>
        <nav>
            <ul>
                <a href="#">
                    <li>CHARACTERS</li>
                </a>
                <a href="#">
                    <li>COMICS</li>
                </a>
                <a href="#">
                    <li>MOVIES</li>
                </a>
                <a href="#">
                    <li>TV</li>
                </a>
                <a href="#">
                    <li>GAMES</li>
                </a>
                <a href="#">
                    <li>COLLECTIBLES</li>
                </a>
                <a href="#">
                    <li>VIDEOS</li>
                </a>
                <a href="#">
                    <li>FANS</li>
                </a>
                <a href="#">
                    <li>NEWS</li>
                </a>
                <a href="#">
                    <li>SHOP</li>
                </a>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {

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
        }
    }
}

img {
    padding: 10px;
}
</style>