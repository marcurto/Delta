<template>
  <footer class="footer">
    <div class="footer__title">
      <p>Taula de Consens pel Delta</p>
    </div>
    <div class="footer__contact">
      <UiList theme="horizontal">
        <li>977 48 06 80 / 652 061 315</li>
        <li>|</li>
        <a href="#">administracio@tauladeconsens.cat</a>
      </UiList>
    </div>
  </footer>
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

.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: auto;
  background-color: variables.$title-blue;
  color: variables.$white;
  padding: 0.8rem 1.5rem;
        font-size: variables.$text-xs;


  p {
    margin: 0rem;
  }

    @media (max-width: 700px) {
       flex-direction: column;
       &__contact{
         font-size: 10px;
       }
    }
}
</style>
