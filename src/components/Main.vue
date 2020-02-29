<template>
  <main>{{ vueNumber }}</main>
</template>

<script>
const number = 2 * 10;
console.log(number);
export default {
  data() {
    return {
      vueNumber: number
    };
  }
};
</script>

<style></style>
