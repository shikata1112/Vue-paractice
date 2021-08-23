<template>
  <div>
    <router-link to="/" class="link" exact-active-class="link--active"
      >Home</router-link
    >
    <router-link to="/users" class="link" active-class="link--active"
      >Users</router-link
    >
    <router-view></router-view>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.link {
  margin-right: 10px;
}
.link--active {
  font-size: 25px;
}
</style>