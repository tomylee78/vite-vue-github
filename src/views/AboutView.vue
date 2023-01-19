<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>

<script>
export default {
  data() {
    return {};
  },
  mounted() {
    this.axios.get("https://randomuser.me/api/").then((response) => {
      console.log(response.data);
    });
  },
};
</script>
