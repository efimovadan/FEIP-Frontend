<template>
  <MyComponent/>
</template>

<script setup>
import MyComponent from './components/MyComponent.vue';
</script>

<style lang="scss">
:root {
  --font-title: "Open sans", sans-serif;
  --font-text: Montserrat, sans-serif;

   font-family: var(--font-text);
}

html,
body,
#__nuxt {
  height: 100%;
}

body {
  margin: 0px;
}
</style>
