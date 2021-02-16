<template>
  <section>
    <CoverBackground theme="delta">
      <Overally theme="delta">
        <Cover title="EL DELTA DE L'EBRE" theme="delta"/>
      </Overally>
    </CoverBackground>
    <DeltaDescription />
  </section>
</template>

<script>
import CoverBackground from "@/components/ui/atoms/CoverBackground.vue";
import Cover from "@/components/ui/molecules/Cover.vue";
import Overally from "@/components/ui/atoms/Overally.vue";
import DeltaDescription from "@/components/delta/DeltaDescription.vue";

export default {
  layout: "default",
  components: {
    CoverBackground,
    Cover,
    Overally,
    DeltaDescription
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
