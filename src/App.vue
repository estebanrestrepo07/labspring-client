<template>
  <div>
    <navbar></navbar>
    <router-view></router-view>
  </div>
</template>

<script>
  import Navbar from "./components/navbar.vue";
  export default {
    name: 'app',
    components: {
      Navbar
    }
  }


</script>
