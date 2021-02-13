<template>
  <section class="taula-estrategies">
    <div class="taula-estrategies__column">
      <div class="taula-estrategies__image">
        <img src="~static/img/morfologia.png" />
      </div>
      <div class="taula-estrategies__text">
        <h4>MORFOLOGIA</h4>
        <p>
          Caldria mantenir la morfologia del Delta de l’Ebre tant com sigui
          possible. No és acceptable el retrocés com a actuació aïllada que no
          vagi més enllà.
        </p>
      </div>
    </div>
    <div class="taula-estrategies__column">
      <div class="taula-estrategies__image">
        <img src="~static/img/sediments.png" />
      </div>
      <div class="taula-estrategies__text">
        <h4>RESTABLIMENT SEDIMENTS</h4>
        <p>
          Es veu com a solució estructural, és a dir, aquella que si no es duu a
          terme, difícilment donarà valor en el temps a les altres possibles
          mesures. Es constata que els seus efectes es preveuen a mitjà i llarg
          termini.
        </p>
      </div>
    </div>
    <div class="taula-estrategies__column">
      <div class="taula-estrategies__image">
        <img src="~static/img/altres.png" />
      </div>
      <div class="taula-estrategies__text">
        <h4>ALTRES MESURES</h4>
        <p>
          S’entenen com a mesures urgents a efectuar a curt termini. Es constata
          l’acceptació de la seva diversificació, és a dir, aplicar diferents
          actuacions segons la tipologia de zona a protegir i segons la gravetat
          de la situació.
        </p>
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

.taula-estrategies {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: space-around;
  padding: 3rem 2rem 5rem;
  text-align: center;
  flex-wrap: wrap;

  &__column {
    width: 33%;
    padding: 0rem 2rem;
  }

  &__image {
    padding-bottom: 2rem;
    img {
      height: 13rem;
      width: auto;
    }
  }

  &__text{
    p{
      text-align: justify;
    }
  }

  @media (max-width: 1130px) {
    &__column {
      padding: 0.5rem;
    }

    img {
      height: 10rem;
    }

    h4 {
      font-size: variables.$text;
    }

    p {
      font-size: variables.$text-s;
    }
  }

  @media (max-width: 700px) {
    flex-direction: column;
    width: 100%;
    align-items: center;

    &__column{
      width: 100%;
    }
  }
}
</style>
