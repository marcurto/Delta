<template>
  <section>
     <CoverBackground theme="contacta">
      <Overally>
        <Cover title="CONTACTA" subtitle="CONTACTA AMB NOSALTRES I ESTAREM ENCANTATS D'ATENDRE QUALSEVOL DUBTE"/>
      </Overally>
    </CoverBackground>
    <ContactaMain/>

  </section>
</template>

<script>
import CoverBackground from "@/components/ui/atoms/CoverBackground.vue";
import ContactaMain from "@/components/contacta/ContactaMain.vue";
import Cover from "@/components/ui/molecules/Cover.vue";
import Overally from "@/components/ui/atoms/Overally.vue";
import Footer from "@/components/common/Footer.vue";


export default {
  layout: "default",
  components: {
    CoverBackground,
    Cover,
    Overally,
    ContactaMain,
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
