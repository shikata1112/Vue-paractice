<template>
  <div>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
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