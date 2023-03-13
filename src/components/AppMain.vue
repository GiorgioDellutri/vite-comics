<script>
import ComicsComponent from './ComicsComponent.vue';

export default {
    name: "ComicsSeries",
    components: {
        ComicsComponent
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://m.media-amazon.com/images/I/51f+H6WXoCL.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.comicsbox.it/cover_dc/AQUAMANNUA_001.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://i.ebayimg.com/images/g/AdwAAOSwcDZhbpfw/s-l500.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.fumetto-online.it/ew/ew_albi/images/PLAY%20PRESS/BATMAN_MAGAZINE001.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.animeclick.it/immagini/anime/Batman_Beyond/cover/Batman_Beyond-cover.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://image.keycollectorcomics.com/media/b1603054384721superman_batman_mag.png",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.starshop.it/media/catalog/product/cache/7529cec0f5c016a97e93cd52e8599a75/p/r/prodotti-00002BMMA0017.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "http://i2.wp.com/batman-news.com/wp-content/uploads/2015/10/Jared-Leto-Empire-Hi-res.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://cdn.shopify.com/s/files/1/0073/0028/4487/products/ThreeJokers2_610x.jpg?v=1602817518",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.fumetto-online.it/ew/ew_albi/images/PLAY%20PRESS/BATMAN_MAGAZINE001.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        };
    },
}
</script>

<template>
    <div class="jumbotron">
    </div>
    <div class="main-container">
        <section class="content-banner wrapper">
            <div class="tag-series">
                <a href="#">
                    <h4>Current Series</h4>
                </a>
            </div>
            <div class="comics">
                <ComicsComponent v-for="comicElement in comics" :thumb="comicElement.thumb" :price="comicElement.price"
                    :series="comicElement.series" :type="comicElement.type" />
            </div>
            <div class="more-button">
                <a href="#">
                    <h4>Load More</h4>
                </a>
            </div>
        </section>
    </div>
    <nav class="blue-banner"></nav>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

div.jumbotron {
    height: 400px;
    background-image: url(../assets/jumbotron.jpg);
    background-size: cover;
}

.main-container {
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    align-items: center;
    background-color: $nav-main-color;
}

.content-banner {
    padding-bottom: 2rem;
    align-items: center;

    div.comics {
        display: flex;
        flex-wrap: wrap;
    }

    div.more-button,
    div.tag-series {

        text-align: center;
        margin: 0 auto;
        width: 190px;
        background-color: $blue-banner;
    }

    h4 {
        margin-top: 2rem;
        text-transform: uppercase;
        padding: 1rem;
        color: $white-text-color;
    }

    div.tag-series {
        width: 250px;
        position: relative;
        top: -66px;
        left: -587px;
    }
}

h4 {
    font-size: 1.4rem
}

.blue-banner {
    height: 160px;
    background-color: $blue-banner;
}
</style>