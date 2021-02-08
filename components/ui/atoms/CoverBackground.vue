<template>
  <section :class="`cover-background cover-background--${theme}`">
      <slot />
  </section>
</template>

<script>
import Overally from "@/components/ui/atoms/Overally.vue";


export default {
  props: {
    source: {
      type: String,
      default: "~static/img/taula.jpg",
    },
    theme: {
      type: String,
      default: null,
      validator(value) {
        const themes = ["pla", "delta"];
        return themes.includes(value);
      },
    },
  },
  components: {
    Overally
  }
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";

.cover-background {
  height: 100vh;
  width: 100vw;
  top: 0;
  left: 0;
  background-image: url("~static/img/taula.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  &--pla{
    background-image: url("~static/img/pla.jpg");
  }

  &--delta{
    background-image: url("~static/img/delta.jpg");
  }
}
</style>