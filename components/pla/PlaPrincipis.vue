<template>
  <section class="principis">
    <Overally theme="banner">
      <div class="principis__title">
        <h3>PRINCIPIS DE LES ESTRATÈGIES I LES INTERVENCIONS</h3>
        <p>Assumint les recomanacions sobre la gestió integrada de les zones costaneres a Europa, la gestió del Delta de l’Ebre s’hauria de dur a terme sobre la base de:</p>
      </div>
      <div class="principis__items">
        <div>
          <h4></h4>
          <p></p>
        </div>
          <div>
          <h4></h4>
          <p></p>
        </div>
          <div>
          <h4></h4>
          <p></p>
        </div>
          <div>
          <h4></h4>
          <p></p>
        </div>
          <div>
          <h4></h4>
          <p></p>
        </div>
          <div>
          <h4></h4>
          <p></p>
        </div>
          <div>
          <h4></h4>
          <p></p>
        </div>
          <div>
          <h4></h4>
          <p></p>
        </div>
        

      </div>
    </Overally>
  </section>
</template>

<script>
import Banner from "@/components/ui/molecules/Banner.vue";
import Overally from "@/components/ui/atoms/Overally.vue";


export default {
  layout: "default",
  components: {
    Banner,
    Overally
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.principis {

  &__title{
    text-align: center;
    width: 100%;
    p{margin-top: 0rem;}
  }
}
</style>
