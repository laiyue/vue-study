<template>
<div>
    <tab-bar></tab-bar>
    <br>
    <br>
    <swiper-list></swiper-list>
    <content-list></content-list>
    <bottom-menu></bottom-menu>
</div>

</template>
<script>
import tabBar from "../components/tab-bar.vue";
import bottomMenu from "../components/bottom-menu.vue";
import contentList from "../components/content-list.vue";
import swiperList from '../components/swiper-list.vue';
export default {
  name: "App",
  components: {
    tabBar,
    bottomMenu,
    contentList,
    swiperList
  },
};
</script>
