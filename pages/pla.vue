<template>
  <section>
    <CoverBackground theme="pla">
      <Overally theme="pla">
        <Cover title="EL PLA DELTA" subtitle="PROPOSTES D'ACTUACIONS CONSENSUADES DES DEL TERRITORI" theme="pla" />
      </Overally>
    </CoverBackground>
    <PlaDescription />
    <PlaPrincipis/>
    <PlaModel />
    <ZonesIntervencio />
    <Organigrama />
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
import ZonesIntervencio from "@/components/pla/ZonesIntervencio.vue";
import Organigrama from "@/components/pla/Organigrama.vue";
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
    ZonesIntervencio,
    Organigrama,
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
