<template>
  <div class="navbar">
    <div class="navbar__container">
      <h1 class="navbar__container__logo">D</h1>
      <font-awesome-icon icon="fa-solid fa-bars-staggered" class="navbar__container__bars"/>
      <ul class="navbar__container__items">
        <li class="navbar__container__items__item"><a ref="#">Acerca de mi</a></li>
        <li class="navbar__container__items__item"><a ref="#">Experiencia</a></li>
        <li class="navbar__container__items__item"><a ref="#">Trabajos</a></li>
        <li class="navbar__container__items__item"><a ref="#">Contacto</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheNavbar',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  .navbar {
    background-color: $blackberry;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 50px;
    // border: 5px solid;
    &__container {
      width: 95%;
      max-width: 960px;
      display: flex;
      justify-content: space-between;
      color: $white;
      display: flex;
      align-items: center;
      &__bars {
        font-size: 30px;
        padding: 5px;
        &:hover {
          color: $purple;
        }
        @include since (600px) {
          visibility: hidden;
        }
      }
      &__logo {
        font-family: $ff-0;
        font-size: 25px;
        margin-left: 10px;
      }
      &__items {
        // border: 1px solid wheat;
        list-style: none;
        display: none;
        overflow: auto;
        @include since (600px){
          display: flex;
        }
        &__item {
          font-family: $ff-2;
          font-size: 13px;
          // border: 1px solid wheat;
          padding: 10px;
          &:hover {
            color: $purple;
          } 
        }
      }
    }
  }
</style>
