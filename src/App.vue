<template>
  <div id="app">
    <p v-if="ok">OK！</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ok: true,
    };
  },
};
</script>