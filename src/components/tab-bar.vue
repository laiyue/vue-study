<template>
  <div class="nav">
    <ul class="nav-list">
      <li class="nav-item" v-for="item in datas" :key="item.title">
        {{ item.title }}
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      datas: [
        { id: 1, title: "悬疑" },
        { id: 2, title: "都市" },
        { id: 3, title: "都市" },
        { id: 4, title: "言情" },
        { id: 5, title: "历史" },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.nav {
  background: #f7fbfa;
  width: 100%;
  top: 0;
  position: fixed;
  z-index: 999;
  .nav-list {
    width: 100%;
    display: flex;
    justify-content: center;
    .nav-item {
      flex-grow: 1;
      height: 3rem;
      line-height: 3rem;
      position: relative;
    }
    li::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      width: 0%;
      height: 100%;
      border-bottom: 2px solid #000;
    }
    li:hover::before {
      left: 0;
      width: 100%;
    }
  }
}
</style>