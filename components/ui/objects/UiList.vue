<template>
  <div :class="`ui-list ui-list--${theme}`">
    <slot />
  </div>
</template>

<script>
export default {
  props: {
    theme: {
      type: String,
      default: null,
      validator(value){
        return ["horizontal"]
      }
    }
  },
};
</script>

<style lang="scss">
@use "@/assets/style/settings/_variables.scss";

.ui-list {
  margin: 0;
  padding: 0;
  list-style: none;

  &--horizontal {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    align-items: center;
  }
}
</style>
