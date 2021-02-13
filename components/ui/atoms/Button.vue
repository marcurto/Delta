<template>
 <button type="submit">REGALA TEMPS</button>
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

button {
  letter-spacing: 1px;
  background-color: rgb(250, 250, 250, 0.3);
  border: none;
  cursor: pointer;
  font-size: 1.2rem;
  color: rgb(41, 38, 38);
  padding: 0.7rem 1rem;
  transition-duration: 0.3s;
  margin: 1rem;

  &:hover {
    letter-spacing: 1.5px;
    color: rgb(250, 250, 250, 0.7);
  }
}
</style>