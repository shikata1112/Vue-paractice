<template>
  <div id="app">
    <button @click="changeText">切り替え</button>
    <p v-if="ok">OK！</p>
    <p v-else>Not OK...</p>
    <ul>
      <li v-for="fruit in fruits" :key="fruit">{{ fruit }}</li>
    </ul>
    <p>いいね({{ number }})</p>
    <LikeNumber />
  </div>
</template>

<script>
import LikeNumber from "./LikeNumber";

export default {
  components: {
    LikeNumber,
  },
  data() {
    return {
      ok: true,
      fruits: ["aaa", "bbb", "cccc", "dddd"],
      number: 5,
    };
  },
  methods: {
    changeText() {
      this.ok = !this.ok;
    },
  },
};
</script>