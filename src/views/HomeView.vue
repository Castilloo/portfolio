<template>
  <div class="home">
    <the-navbar msg="Welcome to Your Vue.js App"/>
    <presentation />
  </div>
</template>

<script>
// @ is an alias to /src
import TheNavbar from '@/components/TheNavbar.vue';
import Presentation from '@/components/Presentation.vue';

export default {
  name: 'HomeView',
  components: {
    TheNavbar,
    Presentation
  }
}
</script>
