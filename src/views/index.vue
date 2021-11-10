<template>
  <router-link to="/about">Go to About</router-link>
  <div>
    <tab-bar></tab-bar>
  </div>
</template>
<script>
import TabBar from '../components/tabbar.vue'
export default {
  name: "App",
  components: {
    TabBar
  },
};
</script>
