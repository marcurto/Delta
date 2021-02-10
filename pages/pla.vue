<template>
  <section>
    <CoverBackground theme="pla">
      <Overally theme="pla">
        <Cover title="EL PLA DELTA" theme="pla" />
      </Overally>
    </CoverBackground>
    <PlaDescription />
    <PlaPrincipis/>
    <PlaModel />
    <Footer />
  </section>
</template>

<script>
import CoverBackground from "@/components/ui/atoms/CoverBackground.vue";
import Cover from "@/components/ui/molecules/Cover.vue";
import Overally from "@/components/ui/atoms/Overally.vue";
import PlaDescription from "@/components/pla/PlaDescription.vue";
import PlaPrincipis from "@/components/pla/PlaPrincipis.vue";
import PlaModel from "@/components/pla/PlaModel.vue";
import Footer from "@/components/common/Footer.vue";

export default {
  layout: "default",
  components: {
    CoverBackground,
    Cover,
    Overally,
    PlaDescription,
    PlaPrincipis,
    PlaModel,
    Footer,
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
