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
        const themes = ["pla", "delta", "banner" , "contacta"];
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

  &--delta{
    background-color: variables.$brown-overally;
  }

  &--banner{
    background-color: rgba(52, 56, 65, 0.78);
    height: 100%;
    width: 100%;
  }

  &--contacta{
     height: 100%;
    width: 100%;
  }
}
</style>