<template>
  <div class="news">
    <div class="news__image">
      <img :src="`${imagen}`" />
    </div>
    <div class="news__main">
      <div class="news__dades">
        <div class="news__dades__top">
          <img :src="`${logo}`" />
          <h4>{{ date }}</h4>
        </div>
        <div class="news__dades__bottom">
          <!-- <Tag /> -->
        </div>
      </div>
      <div class="news__titles">
        <h4>{{ title }}</h4>
        <p>{{ sutitle }}</p>
      </div>
      <div class="news__share">
        <a :href="`${href}`" target="_blank">Saber més</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imagen: {
      type: String,
      default: "LA TAULA DE CONCENS",
    },
    logo: {
      type: String,
      default: "PROPOSTES D'ACTUACIONS CONSENSUADES DES DEL TERRITORI",
    },
    date: {
      type: String,
      default: "11-01-2021",
    },
     title: {
      type: String,
      default: "La disputa entre la Generalitat i el Ministeri bloqueja el pla de xoc per salvar el Delta de l'Ebre",
    },
      subtitle: {
      type: String,
      default: "El Delta preocupa i molt, sobretot des que el temporal Gloria primer i el Filomena després, van posar sota el focus mediàtic els problemes endèmics que arrossega des de fa molts anys: la regressió permanent, el trencament de l’istme del Trabucador, la subsidència de la plana deltaica i per governar-los a tots, com a la pel·lícula, el que és potser el principal problema estructural esperona la resta: la manca de sediments.Avui hem parlat amb Rafa Sánchez, director tècnic i portaveu de la Taula de Consens.",
    },
      href: {
      type: String,
      default: "https://deltacat.cat/2021/01/29/entrevista-a-rafa-sanchez-director-tecnic-i-portaveu-de-la-taula-de-consens-29-01-2021/",
    },
  },
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.news {
}
</style>