<template>
    <section class="presentation">
        <h4 class="presentation__hello">Hola mi nombre es...</h4>
        <h1 class="presentation__name">xxxxxxxxxx xxxxxx</h1>
        <h2 class="presentation__ocupation">xxxxxxx xxxxxxx</h2>
        <p class="presentation__text"> 
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non doloremque enim unde placeat. Quaerat fuga dolores ratione facere accusantium quis sit maxime, quo vero magnam veritatis iste aut et iusto?
        </p>
    </section>
</template>

<script>
    export default {
        name: "Presentation"
    }
</script>

<style lang="scss" scoped>
    .presentation {
        width: 100%;
        height: fit-content;
        color: $gray;
        font-family: $ff-3;
        padding: 2em 3em;
        min-width: 300px;
        text-justify:distribute-all-lines;
        &__hello {
            font-size: 1.1em;
            font-family: $ff-2;
            font-weight: lighter;
            padding-bottom: 15px;
            color: $white;
        }
        &__name {
            font-family: $ff-1;
            font-size: 2.5em;
            text-transform: uppercase;
            color: $white;
        }
        &__ocupation {
            font-family: $ff-2;
            font-size: 2em;
        }
    }
</style>