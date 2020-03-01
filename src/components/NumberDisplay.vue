<template>
  <main>
    <h2>{{ number }} {{double}}</h2>
    <button @click="valueIncrement(1)"></button>
    <button @click="add(2)">add</button>
    <button @click="numberIncrement(number)">+1</button>
    <button @click="numberDecrement(2)">-1</button>
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
  computed: {
    double() {
      return this.number * 2;
    }
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
    valueIncrement(value) {
      return value++;
    },
    numberIncrement() {
      return this.number++;
    },
    numberDecrement() {
      return this.number--;
    },
    add(value) {
      return (this.number = this.number + value);
    }
  }
};
</script>

<style>
button {
  margin: 0 10px;
}
</style>
