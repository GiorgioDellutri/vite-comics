<template>
    <div class="footer-container">
        <section class="info wrapper">
            <div>
                <h1>Dc Comics</h1>
                <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>Tv</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li></li>
                </ul>
                <h1>Shop</h1>
                <ul>
                    <li>Shop</li>
                    <li>Shop DC Collectibles</li>
                </ul>
            </div>

        </section>
        <section class="social">

        </section>
    </div>

</template>

<script>
export default {

}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.footer-container {
    height: 450px;
    background-image: url(../assets/footer-bg.jpg);

    .info {
        height: 450px;
        padding: 1.6rem;

        h1 {
            color: $white-text-color;
            text-transform: uppercase;
        }

        ul li {
            color: $list-text-footer-color;
            margin-left: 0;
        }
    }
}

.social {
    height: 100px;
    background-color: $footer-second-bgcolor ;
}
</style>