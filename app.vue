<template>
  <Header/>
  <Content/>
  <Footer/>
</template>

<script setup>
import Header from '~/components/Header.vue'
import Content from '~/components/Content.vue'
import Footer from '~/components/Footer.vue'
</script>

<style lang="scss">
:root {
  --font-title: "Open sans", sans-serif;
  --font-text: Montserrat, sans-serif;

   font-family: var(--font-text);
}

body {
  margin: 0px;
}
</style>
