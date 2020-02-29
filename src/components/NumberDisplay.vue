<template>
  <main>
    <button @click="incrementer()">{{ name }}</button>
    <button @click="incrementer2(2)">{{ name }}2</button>
    <button @click="incrementer2(vueNumber)">{{ name }}3</button>
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
    incrementer() {
      alert(this.vueNumber);
    },
    incrementer2(value) {
      alert(value);
    }
  }
};
</script>

<style>
button {
  margin: 0 10px;
}
</style>
