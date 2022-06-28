<template>
  <div>
    <h1>{{ msg }}</h1>
    <h2>{{ obj.name }}</h2>
    <h3>{{ obj.age >= 18 ? '成年' : '未成年' }}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: 'HelloWorld',
      obj: {
        name: 'vv',
        age: 18,
      },
    };
  },
};
</script>

<style scoped></style>
