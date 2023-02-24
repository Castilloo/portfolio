<template>
  <nav class="navbar">
    <aside class="navbar__options" v-show="optionsActived">
      <ul class="navbar__options__items">
        <li class="navbar__options__items__item">Acerca de mi</li>
        <li class="navbar__options__items__item">Experiencia</li>
        <li class="navbar__options__items__item">Trabajos</li>
        <li class="navbar__options__items__item">Contacto</li>
      </ul>
    </aside>
    <div class="navbar__container">
      <h1 class="navbar__container__logo">D</h1>
      <div class="navbar__container__bars" @click="toggleOptions">
        <i class="navbar__container__bars fa fa-bars"></i>
      </div>
      <ul class="navbar__container__items">
        <li class="navbar__container__items__item"><a ref="#">Acerca de mi</a></li>
        <li class="navbar__container__items__item"><a ref="#">Experiencia</a></li>
        <li class="navbar__container__items__item"><a ref="#">Trabajos</a></li>
        <li class="navbar__container__items__item"><a ref="#">Contacto</a></li>
      </ul>
    </div>

  </nav>
</template>

<script>
export default {
  name: 'TheNavbar',
  data() {
    return {
      optionsActived: null,
      isMobile: null,
      windowWidth: null
    }
  },
  created() {
    window.addEventListener('resize', this.checkScreen);
    this.checkScreen;
  },
  methods: {
    toggleOptions() {
      this.optionsActived = !this.optionsActived;
      if ()
    },
    checkScreen() {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth <= 600) return this.isMobile = true;
      this.isMobile = true;
    }
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
    &__options {
      background-color: $blackberry;
      width: 100%;
      display: flex;
      justify-content: center;
      position: fixed;
      top: 50px;
      left: 0;
      &__items {
        width: 60%;
        border-top: 2px solid $purple; 
        list-style: none;
        min-width: 200px;
        &__item {
        margin: 20px 0;
          font-family: $ff-2;
          text-align: center;
          padding: 10px;
          color: $white;
        }
      }
    }
    &__container {
      width: 95%;
      max-width: 960px;
      display: flex;
      justify-content: space-between;
      color: $white;
      display: flex;
      align-items: center;
      &__bars {
        &:hover {
          color: $purple;
        }
        & fa .fa-bars{
          font-size: 30px;
          padding: 5px;
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
