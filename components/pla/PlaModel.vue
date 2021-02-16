<template>
  <section class="description">
    <div class="description__left">
      <div class="description__left__text">
        <h3>EL MODEL INTEGRAT DE DEFENSA</h3>
        <p>
          A més del retorn al riu dels sediments retinguts als embassaments,
          caldrà la posada en pràctica d'altres mesures per solucionar els
          problemes urgents i a mitjà termini que pateix la costa deltaica. És
          per això que en el context específic del Delta es proposa un model
          integrat de defensa aplicant diferents actuacions segons la tipologia
          de zona a protegir i segons la gravetat de la situació.
        </p>
      </div>
    </div>

    <div class="description__right">
      <!-- <div class="description__right__list">
        <UiList theme="horizontal" class="description__right__main">
          <div>
            <li>1. Aportació de sorres</li>
            <li>2. Creació i reformació de dunes</li>
            <li>3. Creació de zones humides</li>
          </div>
          <div>
            <li>4. Mota interior (camí de guarda)</li>
            <li>5. Defenses al medi marí</li>
          </div>
        </UiList>
        <div class="description__right__image">
          <img src="~static/img/perfil.png" />
        </div>
      </div> -->
      <img src="~static/img/listaperfil.png" />
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
  background-color: variables.$gray;
  height: 100%;
  width: 100%;
  display: flex;
  margin-top: 3rem;

  &__left {
    height: 100%;
    width: 40%;
    display: flex;
    flex-direction: column;
    align-items: center;

    &__text {
      padding: 4rem;
      text-align: justify;
    }
  }

  &__right {
    height: 100%;
    width: 60%;
    padding: 4rem 0rem;

    img {
      position: relative;
    }

    &__list {
      background-color: variables.$title-green;
      width: 100%;
      padding: 4rem;
    }

    &__main {
      color: variables.$white;
      display: flex;
      justify-content: space-around;
      align-items: flex-start;

      li {
        margin-bottom: 0.4rem;
      }
    }

    &__image {
      background-color: variables.$white;
      padding: 1rem;
    }
  }

  @media (max-width: 1000px) {
    flex-direction: column;

    &__left {
      width: 100%;
      &__text {
        padding: 1rem;
      }
    }

    &__right {
      width: 100%;
    }
  }

  @media (max-width: 780px) {
    padding: 1rem 3rem;
  }

  @media (max-width: 700px) {
    padding: 2rem;

    &__right {
      padding: 0rem;
    }
  }

  @media (max-width: 500px) {
    h3 {
      font-size: variables.$subtitle;
    }
  }
}
</style>
