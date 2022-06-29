<template>
  <div>
    <h1>{{ msg }}</h1>
    <button @click="btn">反转</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: 'Hello,World',
    };
  },
  methods: {
    btn() {
      this.msg = this.msg.split('').reverse().join('');
    },
  },
};
</script>

<style></style>
