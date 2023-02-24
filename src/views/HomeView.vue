<template>
  <div class="home">
    <the-navbar msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import TheNavbar from '@/components/TheNavbar.vue'

export default {
  name: 'HomeView',
  components: {
    TheNavbar
  }
}
</script>
