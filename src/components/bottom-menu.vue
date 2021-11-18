<template>
  <div class="bottom-menu">
    <ul>
      <li class="bottom-menu-item">
        <a href="">
          <span class="mui-icon-extra mui-icon-extra-lamp"></span>
          <label for="">原创</label>
        </a>
      </li>
      <li class="bottom-menu-item">
        <a href="">
          <span class="mui-icon-extra mui-icon-extra-cart"></span>
          <label for="">购物车</label>
        </a>
      </li>
      <li class="bottom-menu-item">
        <a href="">
          <span class="mui-icon-extra mui-icon-extra-xiaoshuo"></span>
          <label for="">书店</label>
        </a>
      </li>
      <li class="bottom-menu-item">
        <a href="">
          <span class="mui-icon-extra mui-icon-extra-peoples"></span>
          <label for="">我的</label>
        </a>
      </li>
      <li class="bottom-menu-item">
        <a href="">
          <span class="mui-icon-extra mui-icon-extra-find"></span>
          <label for="">本地</label>
        </a>
      </li>
    </ul>
  </div>
</template>
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
      a{
        display: flex;
        flex-direction: column;
        padding: 0.5rem 0rem;
        span {
          height: 2rem;
          line-height: 2rem;
        }
        label {
          line-height: 2rem;
          height: 2rem;
        }
      }
    }
  }
}
</style>