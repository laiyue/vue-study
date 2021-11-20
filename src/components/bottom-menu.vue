<template>
  <div class="bottom-menu">
    <ul>
      <li class="bottom-menu-item" v-for="item in datas" :key="item.title">
        <a href="">
          <span class="mui-icon-extra" :class="item.icon"></span>
          <label for="">{{ item.title }}</label>
        </a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      datas: [
        { title: "原创", icon: "mui-icon-extra-lamp" },
        { title: "购物车", icon: "mui-icon-extra-cart" },
        { title: "书店", icon: "mui-icon-extra-xiaoshuo" },
        { title: "我的", icon: "mui-icon-extra-peoples" },
        { title: "本地", icon: "mui-icon-extra-find" },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.bottom-menu {
  width: 100%;
  bottom: 0px;
  position: fixed;
  background: #f7fbfa;
  ul {
    width: 100%;
    flex-grow: 1;
    display: inline-flex;
    align-items: center;
    li {
      flex-grow: 1;
      a {
        display: flex;
        flex-direction: column;
        padding: 0.5rem 0rem;
        span {
          height: 1.5rem;
          line-height: 1.5rem;
        }
        label {
          line-height: 1.5rem;
          height: 1.5rem;
        }
      }
    }
  }
}
</style>
