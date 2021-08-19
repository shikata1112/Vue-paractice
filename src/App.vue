<template>
  <div id="app">
    <button @click="changeText">切り替え</button>
    <p v-if="ok">OK！</p>
    <p v-else>Not OK...</p>

    <ul>
      <li v-for="fruit in fruits" :key="fruit">{{ fruit }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ok: true,
      fruits: ["aaa", "bbb", "cccc", "dddd"],
    };
  },
  methods: {
    changeText() {
      this.ok = !this.ok;
    },
  },
};
</script>