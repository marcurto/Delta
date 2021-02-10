<template>
  <div id="navigation-mobile">
    <UiList>
      <li><i class="fas fa-times" @click="callback()"></i></li>
      <li @click="move('taula')">La Taula de Concens</li>
      <li @click="move('pla')">El Pla Delta</li>
      <li @click="move('delta')">El Delta de l'Ebre</li>
      <li @click="move('premsa')">Sala de Premsa</li>
      <li @click="move('contacta')">Contacta</li>
    </UiList>
  </div>
</template>

<script>
import UiList from "@/components/ui/objects/UiList.vue";

export default {
  components: {
    UiList,
  },
  methods: {
    move(route) {
      this.$props.callback();
      this.$router.push(route);
    },
  },
  props: {
    callback: {
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");

#navigation-mobile {
  position: absolute;
  background-color: variables.$white-overally;
  top: 0;
  left: 0;
  height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;

  li {
    color: black;
    font-size: variables.$title-m;
    text-align: center;
    margin: 1.5rem;
    text-transform: uppercase;
    transition-duration: 0.5s;
    font-family: variables.$font-family-titles;

    i {
      font-size: variables.$title-s;
    }

    &:hover {
      color: variables.$logo;
      cursor: pointer;
      letter-spacing: 0.5px;
    }

    @media (max-width: 700px) {
      font-size: variables.$subtitle;
    }

    @media (min-width: 2000px) {
      font-size: variables.$title;
    }
  }
}
</style>
