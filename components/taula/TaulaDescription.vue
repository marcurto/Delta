<template>
  <section class="description">
    <img src="~static/img/logo-big-dos.png" />
    <div></div>
    <div class="description__main">
      <h3>QUÈ ÉS LA TAULA DE CONCENS?</h3>
      <p>
        La Taula de consens és una entitat del Delta de l’Ebre que té com a
        finalitat la salvaguarda del Delta de l’Ebre davant la greu problemàtica
        que representa la seva continuada desaparició física.
      </p>
      <p>
        Entre els mesos de maig i juny de 2018 es va efectuar una ronda de
        consultes entre els Municipis del Delta i les dues Comunitats de Regants
        per definir la pròpia entitat i els seus objectius. En data 17 de juliol
        de 2018 acorden sotmetre als seus plenaris i assemblees generals
        corresponents el Document de Consens i Territori. per tal que se li doni
        recolzament i es ratifiqui.
      </p>
      <p>
        Entre els mesos de maig i juny de 2018 es va efectuar una ronda de
        consultes entre els Municipis del Delta i les dues Comunitats de Regants
        per definir la pròpia entitat i els seus objectius. En data 17 de juliol
        de 2018 acorden sotmetre als seus plenaris i assemblees generals
        corresponents el Document de Consens i Territori. per tal que se li doni
        recolzament i es ratifiqui.
      </p>
      <p>
        La Taula de consens és una entitat del Delta de l’Ebre que té com a
        finalitat la salvaguarda del Delta de l’Ebre davant la greu problemàtica
        que representa la seva continuada desaparició física.
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
  padding: 3rem 4rem;
  background-color: variables.$background-blue;
  display: grid;
  grid-template-columns: 1fr 2.5fr;

  &__main{padding: 5rem 0rem;}

  img {
    width: 500px;
    position: absolute;
  }
}
</style>
