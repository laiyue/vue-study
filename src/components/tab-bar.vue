<template>
  <div class="nav">
    <ul class="nav-list">
      <li class="nav-item">悬疑</li>
      <li class="nav-item">都市</li>
      <li class="nav-item">职业</li>
      <li class="nav-item">言情</li>
      <li class="nav-item">历史</li>
    </ul>
  </div>
</template>
<style lang="scss" scoped>
.nav {
  background: #f7fbfa;
  width: 100%;
  top: 0px;
  position: fixed;
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
      left:100%;
      width: 0%;
      height: 100%;
      border-bottom: 2px solid #000;
    }
    li:hover::before {
      left: 0;
      width: 100%;
    }
    li:hover ~ li::before {
      left: 0;
    }
  }
}
</style>