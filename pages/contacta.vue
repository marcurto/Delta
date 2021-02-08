<template>
  <section>
    <ContactaLayout/>

  </section>
</template>

<script>

import Footer from "@/components/common/Footer.vue";
import ContactaLayout from "@/components/contacta/ContactaLayout.vue";


export default {
  layout: "default",
  components: {
  
    Footer,
    ContactaLayout
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
