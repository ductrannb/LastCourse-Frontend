<template>
  <div id="content" class="user-not-select">Coming soon</div>
</template>

<script>
import DefaultLayout from "../Layouts/DefaultLayout.vue";
export default {
  name: "ComingSoon",
  components: { DefaultLayout },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Kalam:wght@700&display=swap");

#content {
  width: 100%;
  text-align: center;
  font-family: "Kalam", cursive;
  padding: 48px;
  font-size: 36px;
  font-weight: 700;
  height: 100vh;
}
.main-content {
  padding: 0 !important;
}
</style>
