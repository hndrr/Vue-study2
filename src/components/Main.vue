<template>
  <main>
    <h2 @click="alerter()">{{ name }}</h2>
    <h2 @click="alerter2('aaaaaa')">{{ name }}2</h2>
    <h2 @click="alerter2(vueNumber)">{{ name }}3</h2>
  </main>
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
    },
    alerter2(value) {
      alert(value);
    }
  }
};
</script>

<style></style>
