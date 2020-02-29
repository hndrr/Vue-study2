<template>
  <main>
    <button @click="numberIncrement()">{{ number }}</button>
    <button @click="numberDecrement()">{{ number }}</button>
    <button @click="alerter2(number)">{{ name }}</button>
  </main>
</template>

<script>
const number = 2 * 19;
console.log(number);
export default {
  data() {
    return {
      //ReativeなData
      number: 0,
      name: "hndr"
    };
  },
  methods: {
    numberIncrement() {
      return this.number++;
    },
    numberDecrement() {
      return this.number--;
    },
    alerter() {
      alert(this.number);
    },
    alerter2(value) {
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
