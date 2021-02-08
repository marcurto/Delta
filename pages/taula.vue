<template>
  <section>
    <CoverBackground>
      <Overally>
        <Cover/>
      </Overally>
    </CoverBackground>
  </section>
</template>

<script>
import CoverBackground from "@/components/ui/atoms/CoverBackground.vue";
import Cover from "@/components/ui/molecules/Cover.vue";
import Overally from "@/components/ui/atoms/Overally.vue";

export default {
  layout: "default",
  components: {
    CoverBackground,
    Cover,
    Overally
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

section {
  height: 100%;
}
</style>
