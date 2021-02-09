<template>
  <section>
    <CoverBackground theme="premsa">
      <Overally>
        <Cover title="SALA DE PREMSA"/>
      </Overally>
    </CoverBackground>
    <Years/>
    <News/>
        <News/>

    <Footer />

  </section>
</template>

<script>
import CoverBackground from "@/components/ui/atoms/CoverBackground.vue";
import Cover from "@/components/ui/molecules/Cover.vue";
import Overally from "@/components/ui/atoms/Overally.vue";
import Years from "@/components/premsa/Years.vue";
import News from "@/components/ui/molecules/News.vue";
import Footer from "@/components/common/Footer.vue";


export default {
  layout: "default",
  components: {
    CoverBackground,
    Cover,
    Overally,
    Years,
    News,
    Footer
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
