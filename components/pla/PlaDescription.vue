<template>
  <section class="description">
    <img src="~static/img/siluetadelta.png" />
    <div class="description__blank"></div>
     <div class="description__main">
    <h3>QUÈ ÉS EL PLA DELTA?</h3>
    <p>
      La visió compartida des d’aquest territori contempla i viu el Delta com un
      ecosistema únic, natural i dinàmic, amb biodiversitat característica,
      paisatges oberts i ric patrimoni cultural, un espai del qual gaudeix
      tothom i que proporciona beneficis de forma sostenible a les generacions
      presents i futures.
    </p>
    <p>
      Per això, durant l’any 2019 es va elaborar el Pla Delta, un document
      estratègic que recull i desenvolupa la visió del territori de com afrontar
      el repte de la regressió i la inundació. Finalment, va ser presentat el 28
      de gener de 2020 amb la única finalitat de fer front a les possibles
      conseqüències que pot tenir la no actuació.
    </p>
     </div>
  </section>
</template>

<script>
export default {
  layout: "default",
  components: {},
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.description {
  height: 100%;
  padding: 4rem 4rem;
  background-color: variables.$white;

  &__main {
    padding: 2rem 0rem 2rem 12rem;
    text-align: justify;
  }

  img {
    width: 400px;
    position: absolute;
  }

  @media (max-width: 780px) {
     display: block;
    padding: 1rem 3rem;
    &__blank {
      display: none;
    }
     &__main{
      padding: 2rem;
    }
  }

  @media (max-width: 700px) {
    padding: 2rem;
  }
   @media (max-width: 500px) {
    h3{
      font-size: variables.$subtitle;
    }

   
   }
}
</style>
