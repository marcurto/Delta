<template>
  <component :is="tag" :class="`container container--${theme}`">
    <slot />
  </component>
</template>

<script>
export default {
  props: {
    tag: {
      type: String,
      default: "div",
    },
    theme: {
      type: String,
      default: null,
      validator(value){
        const themes = ["nav"];
        return themes.includes(value);
      }
    }
  },
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";

.container {
  padding: 2rem;
  margin: 0 auto;

  /* &--nav {
    
  } */
}
</style>