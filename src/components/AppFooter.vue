<template>
    <div class="footer-container">
        <div class="footer-wrapper wrapper">
            <section class="info-container">
                <div>
                    <h1>Dc Comics</h1>
                    <ul>
                        <a href="">
                            <li>Characters</li>
                        </a>
                        <a href="">
                            <li>Comics</li>
                        </a>
                        <a href="">
                            <li>Movies</li>
                        </a>
                        <a href="">
                            <li>Tv</li>
                        </a>
                        <a href="">
                            <li>Games</li>
                        </a>
                        <a href="">
                            <li>Videos</li>
                        </a>
                        <a href="">
                            <li>News</li>
                        </a>
                    </ul>
                    <h1>Shop</h1>
                    <ul>
                        <a href="">
                            <li>Shop</li>
                        </a>
                        <a href="">
                            <li>Shop DC Collectibles</li>
                        </a>
                    </ul>
                </div>
                <div>
                    <h1>Dc</h1>
                    <ul>
                        <a href="">
                            <li>Terms Of Use</li>
                        </a>
                        <a href="">
                            <li>Pryvacy policy (New)</li>
                        </a>
                        <a href="">
                            <li>All Choises</li>
                        </a>
                        <a href="">
                            <li>Advertising</li>
                        </a>
                        <a href="">
                            <li>Jobs</li>
                        </a>
                        <a href="">
                            <li>Subscriptions</li>
                        </a>
                        <a href="">
                            <li>Talent Workshops</li>
                        </a>
                        <a href="">
                            <li>CPSC Certificates</li>
                        </a>
                        <a href="">
                            <li>Shop Help</li>
                        </a>
                        <a href="">
                            <li>Contact Us</li>
                        </a>
                    </ul>
                </div>
                <section>
                    <h1>Sites</h1>
                    <ul>
                        <a href="">
                            <li>DC</li>
                        </a>
                        <a href="">
                            <li>MAD Magazine</li>
                        </a>
                        <a href="">
                            <li>DC Kids</li>
                        </a>
                        <a href="">
                            <li>DC Power visa</li>
                        </a>
                    </ul>
                </section>
            </section>
            <div class="img-container">
                <img src="../assets/dc-logo-bg.png" alt="dc logo">
            </div>
        </div>
    </div>
    <section class="social">
        <div class="wrapper">
            <div class="sign-button">
                <h1>sign-up now</h1>
            </div>
            <div class="social-button">
                <h1>follow us</h1>
                <img src="../assets/footer-facebook.png" alt="fb logo">
                <img src="../assets/footer-twitter.png" alt="twitter logo">
                <img src="../assets/footer-youtube.png" alt="ytb logo">
                <img src="../assets/footer-periscope.png" alt="periscope logo">
                <img src="../assets/footer-pinterest.png" alt="pinterest logo">
            </div>
        </div>
    </section>

</template>

<script>
export default {

}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.footer-container {
    background-image: url(../assets/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 450px;

    .footer-wrapper {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .info-container {
        display: flex;
        padding-top: 2rem;

        h1 {
            color: $white-text-color;
            text-transform: uppercase;
            font-size: 1.3rem;
        }

        ul {
            margin-right: 30px;
        }

        ul a li {
            color: $list-text-footer-color;
            margin: .5rem 0;

            &:hover {
                color: $list-text-footer-color-hover;
            }
        }
    }

    img {
        position: relative;
        top: -50px;
    }
}

.social {
    display: flex;
    height: 80px;
    background-color: $footer-second-bgcolor ;
    padding: 1rem;
    z-index: 1;
    position: relative;

    .wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .sign-button {
        border: 3px solid $blue-banner;
        padding: .6rem .9rem;
    }

    h1 {
        text-transform: uppercase;
        color: $white-text-color;
    }

    .social-button {
        display: flex;
        align-items: center;
        justify-content: space-between;

        img {
            padding: .5rem;
        }
    }

    .social-button h1 {
        justify-content: space-between;
        color: $blue-banner;
        padding: 0 2rem;
    }
}
</style>