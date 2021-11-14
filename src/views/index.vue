<template>
<div>
    <tab-bar></tab-bar>
    <content-list></content-list>
    <bottom-menu></bottom-menu>
</div>

</template>
<script>
import TabBar from "../components/tabbar.vue";
import bottomMenu from "../components/bottom-menu.vue";
import ContentList from "../components/content-list.vue";

export default {
  name: "App",
  components: {
    TabBar,
    bottomMenu,
    ContentList,
  },
};
</script>
