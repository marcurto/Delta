<template>
  <footer class="footer">
    <div class="footer__title">
      <img src="~static/img/logo_blanc.png" />
    </div>
    <div class="footer__contact">
      <UiList theme="horizontal">
        <li>977 48 06 80 / 652 061 315</li>
        <li>|</li>
        <a href="mailto:administracio@tauladeconsens.cat"
          >administracio@tauladeconsens.cat<i
            class="fas fa-external-link-alt"
          ></i
        ></a>
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

@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");

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

  &__title {
    display: flex;
    align-items: center;
    height: 100%;

    img {
      width: 100px;
    }
  }

  p {
    margin: 0rem;
  }

  i {
    margin-left: 0.5rem;
    font-size: variables.$text-xs;
  }

  @media (max-width: 700px) {
    flex-direction: column;
    &__contact {
      font-size: 10px;
    }
  }
}
</style>
