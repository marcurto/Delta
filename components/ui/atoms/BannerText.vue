<template>
  <div class="banner-text">
    <h2>{{ title }}</h2>
    <p>{{ subtitle }}</p>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: "LES ESTRATÈGIES FONAMENTALS",
    },
    subtitle: {
      type: String,
      default:
        "Com a conclusions de consens existent en cadascun dels aspectes tractats, podriem assenyalar els més importants i que haurien d’estar inclosos com a estratègies fonamentals de qualsevol Pla Integral de Protecció del Delta.",
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

.banner-text {
  padding: 5rem 7rem;

  p {
    margin-top: 0rem;
  }

  @media (max-width: 1130px) {
    h2 {
      font-size: variables.$title-s;
    }
  }

   @media (max-width: 780px) {
    padding: 3em 4rem;

    p{
      margin: 0rem;
    }
  }
  @media (max-width: 700px) {
    padding: 2rem;
  }
   @media (max-width: 500px) {
    h2{
      font-size: variables.$subtitle;
    }
  }
}
</style>