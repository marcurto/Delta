<template>
  <section class="description">
    <img src="~static/img/logo-big-dos.png" />
    <div class="description__blank"></div>
    <div class="description__main">
      <h3>QUÈ ÉS LA TAULA DE CONSENS?</h3>
      <p>
        La Taula de consens és una entitat que té com a finalitat la salvaguarda
        del Delta de l’Ebre davant la greu problemàtica que representa la seva
        continuada desaparició física.
      </p>
      <p>
        Entre els mesos de maig i juny de 2018 es va efectuar una ronda de
        consultes entre els Municipis del Delta i les dues Comunitats de Regants
        per definir la pròpia entitat i els seus objectius. En data 17 de juliol
        de 2018 acorden sotmetre als seus plenaris i assemblees generals
        corresponents el Document de Consens i Territori per tal que se li doni
        recolzament i es ratifiqui.
      </p>
      <p>
        Aquesta institució està formada pels 7 Ajuntaments de la pròpia plana
        deltaica (Deltebre, Sant Jaume d’Enveja, Sant Carles de la Ràpita,
        Amposta, Camarles, l’Ampolla i l’Aldea), i les dues Comunitats de
        regants (Comunitat de Regants Sindicat Agrícola de l’Ebre i la Comunitat
        General de Regants del Canal de la Dreta de l’Ebre), entitats i
        corporacions transversals, tant pel que fa a la legítima
        representativitat del territori, com pel que fa referència a la
        coneixença de les diferents sensibilitats existents.
      </p>
      <p>
        Fruit de converses i trobades amb diferents actors socials, sectors
        ambientalistes, socioeconòmics i institucionals del territori, sorgeix
        la idea de que sí que és possible arribar a una petició consensuada per
        part del territori per a fer front a la problemàtica del Delta.
      </p>
      <LogosAyuntamientos />
 
    </div>
  
  </section>
</template>

<script>
import LogosAyuntamientos from "@/components/ui/atoms/LogosAyuntamientos.vue";

export default {
  layout: "default",
  components: {
    LogosAyuntamientos
  },
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
  grid-template-columns: 0.5fr 2.5fr;

  &__main {
    padding: 2rem 0rem;
    text-align: justify;
  }

  img {
    width: 600px;
    position: absolute;
  }
 

  @media (max-width: 780px) {
    display: block;
    padding: 1rem 3rem;
    &__blank {
      display: none;
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
