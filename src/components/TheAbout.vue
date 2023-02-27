<template>
    <section class="about">
        <h2 class="about__title">Acerca de mi</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium quas amet assumenda sequi libero accusantium temporibus adipisci iste est illo voluptas earum distinctio perspiciatis suscipit, tenetur non recusandae ipsum perferendis!</p>
    </section>
</template>

<script>
    export default {
        name: 'TheAbout'
    }
</script>

<style lang="scss" scoped>
    .about {
        width: 100%;
        height: fit-content;
        color: $gray;
        font-family: $ff-3;
        padding: 2em 3em;
        min-width: 300px;
        &__title {
            font-family: $ff-2;
            font-weight: bolder;
            text-transform: uppercase;
        }
    }
</style>