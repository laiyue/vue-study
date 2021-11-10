<template>
  <div>
    <tab-bar></tab-bar>
    <bottom-menu></bottom-menu>
  </div>
</template>
<script>
import TabBar from '../components/tabbar.vue'
import bottomMenu from '../components/bottom-menu.vue'
export default {
  name: "App",
  components: {
    TabBar,
    bottomMenu
  },
};
</script>
