<template>
  <div class="home">
    <the-navbar msg="Welcome to Your Vue.js App"/>
    <presentation />
    <the-about />
  </div>
</template>

<script>
// @ is an alias to /src
import TheNavbar from '@/components/TheNavbar.vue';
import Presentation from '@/components/Presentation.vue';
import TheAbout from '@/components/TheAbout.vue';

export default {
  name: 'HomeView',
  components: {
    TheNavbar,
    Presentation,
    TheAbout
  }
}
</script>
