<template>
  <div class="swiper">
    <div class="swiper-wrap">
      <img
        v-for="item in datas"
        class="pic"
        :src="item.pic"
        alt=""
        :key="item.pic"
      />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      datas: [
        { pic: require("../assets/images/7403.jpg") },
        { pic: require("../assets/images/7410.jpg") },
        { pic: require("../assets/images/7465.jpg") },
        { pic: require("../assets/images/7467.jpg") },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.swiper {
  width: 100%;
  margin: 10px 0px;
  overflow: hidden;
  .swiper-wrap {
    margin-top: -10px;
    width: 400%;
    height: 12rem;
    transform: translate(0, 0); /* 初始位置位移 */
    animation: loop 10s linear infinite;
    .pic {
      width: 25%;
      height: 12rem;
    }
  }
}

@keyframes loop {
  0% {
    transform: translate(0, 0);
  }
  20% {
    transform: translate(0, 0);
  } /* 停留1500ms */

  25% {
    transform: translate(-25%, 0);
  } /* 切换500ms 位移-20% */
  45% {
    transform: translate(-25%, 0);
  }

  50% {
    transform: translate(-50%, 0);
  }
  70% {
    transform: translate(-50%, 0);
  }

  75% {
    transform: translate(-75%, 0);
  }
  95% {
    transform: translate(-75%, 0);
  }
  100% {
    transform: translate(0, 0);
  } /* 复位到第一张图片 */
}
</style>