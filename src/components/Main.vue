<template>
  <main @click="alerter()">{{ name }}</main>
</template>

<script>
const number = 2 * 19;
console.log(number);
export default {
  data() {
    return {
      //ReativeなData
      vueNumber: number,
      name: "hndr"
    };
  },
  methods: {
    alerter() {
      alert(this.vueNumber);
    }
  }
};
</script>

<style></style>
