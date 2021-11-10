<template>
  <div class="nav">
    <ul>
      <li>精选</li>
      <li>精选</li>
      <li>精选</li>
      <li>精选</li>
      <li>精选</li>
    </ul>
  </div>
</template>
<style lang="scss" scoped>
.nav {
  background: #f7fbfa;
  display: flex;
  ul {
    flex-grow: 1;
    list-style: none;
    display: inline-flex;
    align-items: center;
    height: 2rem;
    li {
      flex-grow: 1;
      list-style: none;
      height: 1rem;
      line-height: 1rem;
      margin: 1.2rem;
    }
  }
}
</style>