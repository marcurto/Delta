<template>
  <section class="principis">
    <Overally theme="banner">
      <div class="principis__title">
        <h3>PRINCIPIS DE LES ESTRATÈGIES I LES INTERVENCIONS</h3>
        <p>Assumint les recomanacions sobre la gestió integrada de les zones costaneres a Europa, la gestió del Delta de l’Ebre s’hauria de dur a terme sobre la base de:</p>
      </div>
      <div class="principis__items">
        <div>
          <h4>PRESPECTIVA A LLARG TERMINI</h4>
          <p>temàtica i geogràfica) que tingui en compte la interdependència i disparitat dels sistemes naturals i les activitats humanes que tenen incidència al delta de l’Ebre</p>
        </div>
          <div>
          <h4>PRESPECTIVA AMPLIA I GLOBAL</h4>
          <p>temàtica i geogràfica) que tingui en compte la interdependència i disparitat dels sistemes naturals i les activitats humanes que tenen incidència al delta de l’Ebre</p>
        </div>
         <div>
          <h4>PRESPECTIVA AMPLIA I GLOBAL</h4>
          <p>temàtica i geogràfica) que tingui en compte la interdependència i disparitat dels sistemes naturals i les activitats humanes que tenen incidència al delta de l’Ebre</p>
        </div>
         <div>
          <h4>PRESPECTIVA AMPLIA I GLOBAL</h4>
          <p>temàtica i geogràfica) que tingui en compte la interdependència i disparitat dels sistemes naturals i les activitats humanes que tenen incidència al delta de l’Ebre</p>
        </div>
         <div>
          <h4>PRESPECTIVA AMPLIA I GLOBAL</h4>
          <p>temàtica i geogràfica) que tingui en compte la interdependència i disparitat dels sistemes naturals i les activitats humanes que tenen incidència al delta de l’Ebre</p>
        </div>
         <div>
          <h4>PRESPECTIVA AMPLIA I GLOBAL</h4>
          <p>temàtica i geogràfica) que tingui en compte la interdependència i disparitat dels sistemes naturals i les activitats humanes que tenen incidència al delta de l’Ebre</p>
        </div>
         <div>
          <h4>PRESPECTIVA AMPLIA I GLOBAL</h4>
          <p>temàtica i geogràfica) que tingui en compte la interdependència i disparitat dels sistemes naturals i les activitats humanes que tenen incidència al delta de l’Ebre</p>
        </div>
         <div>
          <h4>PRESPECTIVA AMPLIA I GLOBAL</h4>
          <p>temàtica i geogràfica) que tingui en compte la interdependència i disparitat dels sistemes naturals i les activitats humanes que tenen incidència al delta de l’Ebre</p>
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
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/index.scss";

.principis {

  color: variables.$white;
  background-image: url("~static/img/aiguamoll.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position-y: center;
  background-position-x: center;

  &__title{
  padding: 1rem;
    text-align: center;
    width: 100%;
    p{margin-top: 0rem;}
  }
  &__items{
    padding: 1rem;
    text-align: left;
    display: flex;
    flex-wrap: wrap;

    div{
      width: 25%;
      padding: 0rem 1rem;
      margin-bottom: 1rem;
    }

    h4{
      font-size: variables.$item;
    }
  }
}
</style>
