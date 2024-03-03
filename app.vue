<template>
  <h1 class="montserrat, color-blue">Hello, world!</h1>
  <h3 class="open-sans, color-red">Strawberry</h3>
</template>

<script>
console.log("Hello, world!");
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');

.color-red {
  color: rgb(226, 41, 41);
}
.color-blue {
  color: rgb(70, 84, 233);
}
.montserrat {
  font-family: Montserrat;
}

.open-sans {
  font-family: "Open sans";
}
</style>
