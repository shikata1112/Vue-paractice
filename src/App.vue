<template>
  <div id="app">
    <h1>トータルのいいね数</h1>
    <h2>{{ number }}</h2>
    <LikeNumber :total-number="number" @my-click="incrementNumber" />
    <LikeNumber :total-number="number" />
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
      number: 5,
    };
  },
  methods: {
    incrementNumber(event) {
      this.number = event;
    },
  },
};
</script>