<template>
  <div class="banner">
    <Overally theme="banner">
      <BannerText/>
    </Overally>
  </div>
</template>

<script>
import Overally from "@/components/ui/atoms/Overally.vue";
import BannerText from "@/components/ui/atoms/BannerText.vue";

export default {
  props: {
    title: {
      type: String,
      default: "LES ESTRATÈGIES FONAMENTALS",
    },
    subtitle: {
      type: String,
      default:
        "Com a conclusions de concens existent en cadascun dels aspectes tractats, podriem assenyalar els més importants i que haurien d’estar inclosos com a estratègies fonalmentsl de qualsevol Pla Integral de Protecció del Delta.",
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
    Overally,
    BannerText
  }
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.banner {
  width: 100%;
  height: 100%;
  background-image: url("~static/img/banner.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position-x: center;
  background-position-y: center;
  position: relative;
  text-align: center;
  color: variables.$white;
}
</style>