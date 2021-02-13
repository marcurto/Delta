<template>
  <div class="news">
    <div class="news__image">
      <img :src="`${img}`" />
    </div>
    <div class="news__main">
      <div class="news__dades">
        <div class="news__dades__top">
          <img :src="`${logo}`" />
          <h4>{{ date }}</h4>
        </div>
        <div class="news__dades__bottom">
          <Tag />
          <Tag tag="Generalitat"/>
        </div>
      </div>
      <div class="news__titles">
        <h4>{{ title }}</h4>
        <p>{{ subtitle }}</p>
      </div>
      <div class="news__share">
        <a :href="`${href}`" target="_blank"
          >Saber més <i class="fas fa-external-link-alt"></i
        ></a>
      </div>
    </div>
  </div>
</template>

<script>
import Tag from "@/components/ui/atoms/Tag.vue";

export default {
  props: {
    img: {
      type: String,
      default: "/_nuxt/static/img/morfologia.png",
    },
    logo: {
      type: String,
      default: "/_nuxt/static/img/elpais.png",
    },
    date: {
      type: String,
      default: "11-01-2021",
    },
    title: {
      type: String,
      default:
        "La disputa entre la Generalitat i el Ministeri bloqueja el pla de xoc per salvar el Delta de l'Ebre",
    },
    subtitle: {
      type: String,
      default:
        "El Delta preocupa i molt, sobretot des que el temporal Gloria primer i el Filomena després, van posar sota el focus mediàtic els problemes endèmics que arrossega des de fa molts anys.",
    },
    href: {
      type: String,
      default:
        "https://deltacat.cat/2021/01/29/entrevista-a-rafa-sanchez-director-tecnic-i-portaveu-de-la-taula-de-consens-29-01-2021/",
    },
  },
  components: {
    Tag,
  },
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");

.news {
  padding: 3rem 3rem 3rem 5rem;
  display: flex;
  height: 100%;
  align-items: center;
  text-align: justify;

  hr{
    width: 100%;
  }

  &__image {
    width: 30%;
  
  }

  &__main {
    padding-left: 2rem;
    height: 100%;
    align-items: space-between;
    width: 70%;

    p{
      margin-top: 0rem;
    }
  }

  &__dades{
    margin-bottom: 1rem;
  }
  &__dades__top {
    display: flex;
    width: 100%;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 0.5rem;

    img {
      height: 2.5rem;
    }

    h4 {
      font-size: variables.$text;
    }
    
  }

  &__share {
    margin-top: 2rem;
    a {
      color: black;
    }
  }

  @media (max-width: 800px) {
  padding: 1rem 1rem;
  flex-direction: column;

    &__main{
          padding-left: 0rem;
          margin-top: 1.5rem;

    }
    }
}
</style>