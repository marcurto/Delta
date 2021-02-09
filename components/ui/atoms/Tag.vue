<template>
  <span>{{ tag }}</span>
</template>

<script>
export default {
  props: {
    tag: {
      type: String,
      default: "Glòria",
    },
    theme: {
      type: String,
      default: null,
      validator(value) {
        const themes = ["pla", "delta", "banner"];
        return themes.includes(value);
      },
    },
  },
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";

span {
  background-color: variables.$logo;
  color: variables.$white;
  padding: 0.2rem 0.7rem;
  border-radius: 25px;
  margin: 0.5rem 0.5rem 0.5rem 0rem;
  font-size: variables.$text-xs;
}
</style>