<template>
  <section class="estrategies">
    <Overally theme="banner">
      <Banner/>
    </Overally>
  </section>
</template>

<script>
import Banner from "@/components/ui/molecules/Banner.vue";
import Overally from "@/components/ui/atoms/Overally.vue";


export default {
  layout: "default",
  components: {
    Banner,
    Overally
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.estrategies {

}
</style>
