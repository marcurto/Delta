<template>
  <section>
    <CoverBackground>
      <Overally>
        <Cover />
      </Overally>
    </CoverBackground>
    <TaulaDescription />
    <TaulaEstrategiesBanner />
    <TaulaEstrategies />
  </section>
</template>

<script>
import CoverBackground from "@/components/ui/atoms/CoverBackground.vue";
import Cover from "@/components/ui/molecules/Cover.vue";
import Overally from "@/components/ui/atoms/Overally.vue";
import TaulaDescription from "@/components/taula/TaulaDescription.vue";
import TaulaEstrategiesBanner from "@/components/taula/TaulaEstrategiesBanner.vue";
import TaulaEstrategies from "@/components/taula/TaulaEstrategies.vue";

export default {
  layout: "default",
  components: {
    CoverBackground,
    Cover,
    Overally,
    TaulaDescription,
    TaulaEstrategiesBanner,
    TaulaEstrategies
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

section {
  height: 100%;
  color: variables.$title-blue;
}
</style>
