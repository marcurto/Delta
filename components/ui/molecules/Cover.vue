<template>
  <component :is="tag" :class="`cover cover--${theme}`">
    <div>
      <h1>{{ title }}</h1>
      <h4>{{ subtitle }}</h4>
    </div>
    <div>
      <slot />
    </div>
  </component>
</template>

<script>
export default {
  props: {
    tag: {
      type: String,
      default: "div",
    },
    title: {
      type: String,
      default: "LA TAULA DE CONSENS",
    },
    subtitle: {
      type: String,
      default: "LA VEU DEL TERRITORI",
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
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.cover{
  height: auto;
  position: absolute;
  z-index: 2;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  width: 100%;
  color: variables.$title-blue;

  &--pla {
    color: variables.$title-green;
  }

  &--delta{
    color: variables.$title-brown;
  }

  h1 {
    padding: 0rem;
  }

     @media (max-width: 700px) {
     h1{
       font-size: variables.$title-m;
     }

     h4{
       
     }
  }

}
</style>