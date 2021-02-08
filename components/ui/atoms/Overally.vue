<template>
  <div :class="`overally overally--${theme}`">
    <slot />
  </div>
</template>

<script>
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
        const themes = ["pla"];
        return themes.includes(value);
      },
    },
  },
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";

.overally {
  height: 100vh;
  width: 100vw;
  top: 0;
  left: 0;
  background-color: variables.$blue-overally;

  &--pla {
    background-color: variables.$green-overally;
  }
}
</style>