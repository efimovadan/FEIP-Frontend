<template>
    <div class="main-wrapper">
      <Header class="header"/>
      <Content class="main"/>
      <Footer class="footer"/>
    </div>
  </template>

<script>
import Header from './Header.vue';
import Content from './Content.vue';
import Footer from './Footer.vue';
</script>

<style lang="scss" scoped>
.main-wrapper {
    height: 100%;
    display: flex;
    flex-direction: column;
}
.header {
    flex-shrink: 0;
}
.main {
    flex-grow: 1;
}
.footer {
    flex-shrink: 0;
}
</style>