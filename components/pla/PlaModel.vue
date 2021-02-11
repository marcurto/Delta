<template>
  <section class="description">
    <h2>EL MODEL INTEGRAT DE DEFENSA</h2>
    <p>
      A més del retorn al riu dels sediments retinguts als embassaments, caldrà
      la posada en pràctica d'altres mesures per solucionar els problemes
      urgents i a mitjà termini que pateix la costa deltaica. És per això que en
      el context específic del Delta es proposa un model integrat de defensa
      aplicant diferents actuacions segons la tipologia de zona a protegir i
      segons la gravetat de la situació.
    </p>
    <div class="description__grafic">
      <UiList theme="horizontal" class="description__list">
        <li>1. Aportació de sorres</li>
        <li>2. Creació i reformació de dunes</li>
        <li>3. Creació de zones humides</li>
        <li>4. Mota interior (camí de guarda)</li>
        <li>5. Defenses al medi marí</li>
      </UiList>
      <div>
        <img src="~static/img/perfil.png" />
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
  padding: 4rem 4rem;
  background-color: variables.$white;

  &__grafic {
    width: 100%;
    display: flex;
    flex-direction: column;
    text-align: center;
    justify-content: center;
  }

  &__list{
    display: flex;
    text-align: center;
    justify-content: center;
    margin-bottom: 2rem;
  }

  @media (max-width: 780px) {
    padding: 1rem 3rem;
  }

  @media (max-width: 700px) {
    padding: 2rem;
  }
}
</style>
