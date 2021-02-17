<template>
  <footer class="footer-inici">
 <p>Regala-li temps al Delta de l'Ebre abans que desaparegui. Totes les donacions aniran destinades a la Taula de Concens pel Delta. <a>Saber més</a></p>
  </footer>
</template>

<script>
import UiList from "@/components/ui/objects/UiList.vue";

export default {
  components: {
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");


.footer-inici {
  position: fixed;
  bottom: 0;
  width: 100%;
  height: auto;
    background-color: rgb(250, 250, 250, 0.3);

  p{
    margin: 0.5rem 1rem;
    font-weight: 500;
    color: variables.$black;

  }

  a{
    color: variables.$black;
    text-decoration: underline;
  }

   @media (max-width: 900px) {
      p{
        font-size: variables.$text-s;
      }
  }
  @media (max-width: 500px) {
      p{
        font-size: variables.$text-mobile;
        line-height: 0.8rem;
      }
  }
}
</style>
