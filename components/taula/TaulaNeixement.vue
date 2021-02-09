<template>
  <section class="description">
    <div class="description__main">
      <h3>PER QUÈ NEIX LA TAULA DE CONCENS?</h3>
      <p>
        Són nombrosos la quantitat d’estudis que fan referència a la
        problemàtica principal que pateix des de fa dècades el Delta de l’Ebre i
        que pot comportar a la seva desaparició física.
      </p>
      <p>
        Tots som conscients de com es va formar el Delta, quina és la seva
        dinàmica actual i el seu final si es no es prenen mesures. Les cuases
        antropogèniques de las ev avulenrabilitat demanen també accions humanes
        per a la seva correcció. De propostes i plans d’actuació concrets també
        en disposem des de fa dàcades.
      </p>
      <p>
        Esque correspon de manera urgent i persistena a les entitats pròpies del
        territori és la justa demanda a les Administracions epr tal que
        compleixin les lleis que fan referència a la protecció i restauració
        d’aquest espai tan valuós i singular.
      </p>
    <div class="description__images">
      <div class="description__images__column">
        <img src="~static/img/morfologia.png" />
      </div>
      <div class="description__images__column">
        <img src="~static/img/morfologia.png" />
      </div>
    </div>
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
  padding: 3rem 4rem 12rem;
  background-color: variables.$background-blue-dark;
  position: relative;
  text-align: left;

  &__main {
    padding: 5rem 0rem;
    position: relative;
  }

  &__images {
    position: absolute;
    display: flex;
    justify-content: center;
    width: 100%;
    z-index: 9;
    padding: 1rem 0rem;

    &__column {
      margin: 3rem;
      background-color: variables.$background-blue;
      width: 20rem;
      height: 20rem;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    img {
      height: 15rem;
    }
  }
   @media (max-width: 780px) {
     padding: 3rem 4rem 5rem;

     &__images__column{
      width: 25rem;
      height: 10rem;
     }
    img{
      height: 8rem;
    }
  }
}
</style>
