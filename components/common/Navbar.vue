<template>
  <nav class="nav">
    <div class="nav__menu">
      <div>
        <i class="fas fa-bars" @click="showSidebar()"></i>
        <Menu v-if="sidebar" :callback="showSidebar"/>
      </div>
      <p>Taula de Concens pel Delta</p>
    </div>
    <div class="nav__contact">
      <UiList theme="horizontal">
        <li>977 48 06 80 / 652 061 315</li>
        <li>|</li>
        <a href="#">administracio@tauladeconcens.cat</a>
      </UiList>
    </div>
  </nav>
</template>

<script>
import UiList from "@/components/ui/objects/UiList.vue";
import Menu from "@/components/common/Menu.vue";

export default {
  components: {
    UiList,
    Menu,
  },
  data: () => {
    return {
      sidebar: false,
    };
  },
  methods: {
    showSidebar() {
      this.$data.sidebar = !this.$data.sidebar;
    },
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");

.nav {
  @include mixins.space-between;
  width: 100%;
  height: 60px;
  color: variables.$white;
  background-color: transparent;
  position: absolute;
  top: 0;
  padding: 1rem;
  z-index: 9;
  font-size: variables.$text-xs;

  &__menu {
    @include mixins.space-between;

    p{
      margin-left: 1rem;
    }
    i {
      cursor: pointer;
    }
  }
}
</style>
