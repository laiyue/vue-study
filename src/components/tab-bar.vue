<template>
  <div class="nav">
    <ul>
      <li>悬疑</li>
      <li>都市</li>
      <li>职业</li>
      <li>言情</li>
      <li>历史</li>
    </ul>
  </div>
</template>
<style lang="scss" scoped>
.nav {
  background: #f7fbfa;
  width: 100%;
  top: 0px;
  position: fixed;
  ul {
    width: 100%;
    display:flex;
    justify-content: center;
    li {
       flex-grow: 1;
      height: 3rem;
      line-height: 3rem;
    }
  }
}
</style>