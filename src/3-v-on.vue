<template>
  <div>
    <p>你要购买的产品数量 {{ count }}</p>
    <button v-on:click="count++">+1</button>
    <button v-on:click="addFn">+1</button>
    <button v-on:click="addFnn(5)">+5</button>
    <button @click="subFn">-1</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: '',
    };
  },
  methods: {
    addFn() {
      this.count++;
    },
    addFnn(val) {
      this.count += val;
    },
    subFn() {
      this.count--;
    },
  },
};
</script>

<style></style>
