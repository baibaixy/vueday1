<template>
  <div @click="fatherFn">
    <button @click.stop="one">stop阻止事件冒泡</button>
    <a @click.prevent="one" href="http://www.google.com/"
      >prevent阻止事件默认行为</a
    >
    <button @click.once="one">只触发一次事件处理函数</button>
  </div>
</template>

<script>
export default {
  methods: {
    fatherFn() {
      console.log(2);
    },
    one() {
      console.log(1);
    },
  },
};
</script>

<style></style>
