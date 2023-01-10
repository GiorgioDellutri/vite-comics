<template>
    <div class="jumbotron">
    </div>
    <div class="main-container">
        <section class="content-banner wrapper">
            <h1>--> Content goes here</h1>
        </section>
        <nav class="blue-banner"></nav>
    </div>
</template>

<script>
export default {

}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

div.jumbotron {
    height: 400px;
    background-image: url(../assets/jumbotron.jpg);
    background-size: cover;
}

.main-container {
    background-color: $nav-main-color;
}

.content-banner {
    height: 150px;
    display: flex;
    align-items: center;

    h1 {
        color: $white-text-color;
        margin-left: 1rem;
        font-size: 2rem;
    }
}

.blue-banner {
    height: 180px;
    background-color: $blue-banner;

}
</style>