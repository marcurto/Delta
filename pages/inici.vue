<template>
  <section>
    <!-- <video autoPlay="autoplay" loop="loop" class="video" muted>
      <source src="~static/img/portada.m4v" type="video/mp4" />
      Your browser does not support the video tag.
    </video> -->

    <h1>hi</h1>
  </section>
</template>

<script>
import Navbar from "@/components/common/Navbar.vue";

export default {
  layout: "default",
  components: {
    Navbar,
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

section {
  background-color: red;
  height: 100vh;
}
</style>
