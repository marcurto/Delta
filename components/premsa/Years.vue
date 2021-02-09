<template>
  <nav class="years">
    <UiList theme="horizontal">
      <li>2018</li>
      <li >2019</li>
      <li >2020</li>
      <li>2021</li>
    </UiList>
  </nav>
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

.years {
  width: 100%;
  padding-right: 4rem;
  border-bottom: black 2px solid;
  margin-bottom: 2rem;
}
</style>
