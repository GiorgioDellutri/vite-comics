<template>
    <div class="footer-container">
        <div class="footer-wrapper wrapper">
            <section class="info-container">
                <div>
                    <h1>Dc Comics</h1>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h1>Shop</h1>
                    <ul>
                        <li>Shop</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div>
                    <h1>Dc</h1>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Pryvacy policy (New)</li>
                        <li>All Choises</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <section>
                    <h1>Sites</h1>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Power visa</li>
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
        overflow: hidden;

        h1 {
            color: $white-text-color;
            text-transform: uppercase;
            font-size: 1.3rem;
        }

        ul {
            margin-right: 30px;
        }

        ul li {
            color: $list-text-footer-color;
            margin: .5rem 0;
        }
    }

    .img-container {
        overflow: hidden;
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

    .wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .sign-button {
        border: 3px solid $blue-banner;
        padding: 0 .9rem;
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