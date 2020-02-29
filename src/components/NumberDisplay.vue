<template>
  <main>
    <button @click="alerter()">{{ name }}</button>
    <button @click="alerter2(2)">{{ name }}2</button>
    <button @click="alerter3(number)">{{ name }}3</button>
    <button @click="alerter3(2)">{{ name }}3</button>
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
    alerter() {
      alert(this.number);
    },
    alerter2(value) {
      alert(value);
    },
    alerter3(value) {
      console.log(this.numberIncrement(value));
    },
    numberIncrement(value) {
      return value++;
    },
    numberDecrement() {
      return this.number--;
    }
  }
};
</script>

<style>
button {
  margin: 0 10px;
}
</style>
