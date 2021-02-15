<template>
  <section>
    <!-- <CoverBackground theme="delta">
      <Overally theme="delta">
        <CountdownCointainer />
      </Overally>
    </CoverBackground>
    <Video /> -->
  </section>
</template>

<script>
import CountdownCointainer from "@/components/ui/molecules/CountdownContainer.vue";
import CoverBackground from "@/components/ui/atoms/CoverBackground.vue";
import Overally from "@/components/ui/atoms/Overally.vue";
// import Video from "@/components/ui/atoms/Video.vue";


export default {
  layout: "default",
  components: {
    // CountdownCointainer,
    // CoverBackground,
    // Overally,
    // Video
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

section {
  height: 100vh;
}
</style>
