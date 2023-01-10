<script>
export default {
    name: 'ComicsComponent',
    props: [
        'thumb',
        'price',
        'series',
        'type',

    ],
}
</script>

<template>
    <div class="comic-element">
        {{ thumb }} -- {{ price }} -- {{ series }} -- {{ type }}
    </div>
</template>


<style lang="scss">

</style>