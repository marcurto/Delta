<template>
  <div id="navigation-mobile">
    <UiList>
        <li>La Taula de Concens</li>
        <li>El Pla Delta</li>
        <li>El Delta de l'Ebre</li>
        <li>Sala de Premsa</li>
        <li>Contacta</li>
    </UiList>
    <!-- <div class="social-media">
      <i class="fab fa-twitter"></i>
      <i class="fab fa-instagram"></i>
      <i class="fab fa-pinterest"></i>
    </div> -->
  </div>
</template>

<script>
import UiList from "@/components/ui/objects/UiList.vue";

export default {
  components: {
    UiList,
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

#navigation-mobile {
  position: absolute;
  background-color: variables.$white-overally;
  height: 100vh;
  padding: 3rem;

  ul {
    color: black;
  }
}
</style>
