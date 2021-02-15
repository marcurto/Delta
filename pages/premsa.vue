<template>
  <section>
    <CoverBackground theme="premsa">
      <Overally>
        <Cover title="SALA DE PREMSA" />
      </Overally>
    </CoverBackground>
     <nav class="years">
    <UiList theme="horizontal" class="years__list">
      <li @click="toggleComponent = '18'">2018</li>
      <li @click="toggleComponent = '19'">2019</li>
      <li @click="toggleComponent = '20'">2020</li>
      <li @click="toggleComponent = '21'">2021</li>
    </UiList>
  </nav>
    <RecullNoticies18 v-if="toggleComponent === '18'"/>
    <RecullNoticies19 v-if="toggleComponent === '19'"/>
    <RecullNoticies20 v-if="toggleComponent === '20'" />
    <RecullNoticies21 v-if="toggleComponent === '21'"/>
    <Footer />
  </section>
</template>

<script>
import CoverBackground from "@/components/ui/atoms/CoverBackground.vue";
import Cover from "@/components/ui/molecules/Cover.vue";
import Overally from "@/components/ui/atoms/Overally.vue";
import RecullNoticies21 from "@/components/premsa/RecullNoticies21.vue";
import RecullNoticies20 from "@/components/premsa/RecullNoticies20.vue";
import RecullNoticies19 from "@/components/premsa/RecullNoticies19.vue";
import RecullNoticies18 from "@/components/premsa/RecullNoticies18.vue";
import Footer from "@/components/common/Footer.vue";

export default {
  layout: "default",
  components: {
    CoverBackground,
    Cover,
    Overally,
    RecullNoticies21,
    RecullNoticies20,
    RecullNoticies19,
    RecullNoticies18,
    Footer,
  },
  data() {
    return {
      toggleComponent: '21'
    };
  }
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


.years {
  width: 100%;
  margin: 4rem 0rem;

  &__list{
    margin-right: 4rem;
    border-bottom: black 2px solid;
    justify-content: flex-end;

    li{
      margin-right: 1rem;
    }
  }
}
</style>
