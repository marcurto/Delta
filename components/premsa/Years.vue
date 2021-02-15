<template>
  <nav class="years">
    <UiList theme="horizontal" class="years__list">
      <li @click="toggleComponent18">2018</li>
      <li @click="toggleComponent19">2019</li>
      <li @click="toggleComponent20">2020</li>
      <li @click="toggleComponent21">2021</li>
    </UiList>
  </nav>
</template>

<script>
import UiList from "@/components/ui/objects/UiList.vue";
import RecullNoticies21 from "@/components/premsa/RecullNoticies21.vue";
import RecullNoticies20 from "@/components/premsa/RecullNoticies20.vue";
import RecullNoticies19 from "@/components/premsa/RecullNoticies19.vue";
import RecullNoticies18 from "@/components/premsa/RecullNoticies18.vue";


export default {
  components: {
    UiList,
  },
 data() {
    return {
      showComponent18: false,
      showComponent19: false,
      showComponent20: false,
      showComponent21: true
    };
  },
  methods: {
    toggleComponent18 () {
      this.showComponent18 = !this.showComponent18
    },
    toggleComponent19 () {
      this.showComponent19 = !this.showComponent19
    },
    toggleComponent20 () {
      this.showComponent20 = !this.showComponent20
    },
    toggleComponent21 () {
      this.showComponent21 = !this.showComponent21
    },
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");

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
