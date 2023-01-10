<script>
export default {
    name: 'ComicsComponent',
    props:
        [
            'thumb',
            'price',
            'series',
            'type',
        ],
    // {
    //     thumb: String,
    //     price: Number,
    //     series: String,
    //     type: String,
    // },
}
</script>

<template>
    <div class="comic-element">
        <img :src="thumb" alt="thumb image">
        <!-- {{ thumb }} -- {{ price }} -- {{ series }} -- {{ type }} -->
        <p>{{ series }}</p>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

div.comic-element {
    width: calc(100% / 6);
    padding: 1rem;

    img {
        width: 100%;
    }

    p {
        // color: $white-text-color;
        color: white;
        text-transform: uppercase;
    }
}
</style>