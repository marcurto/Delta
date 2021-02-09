<template>
  <div class="news">
    <div class="news__image">
      <img src="~static/img/morfologia.png" />
    </div>
    <div class="news__main">
      <div class="news__dades">
        <div class="news__dades__top">
          <img src="~static/img/elpais.png" />
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
      default: "~static/img/elpais.png",
    },
    logo: {
      type: String,
      default: "hola",
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
  padding: 3rem 3rem 3rem 8rem;
  display: flex;
  height: 100%;
  align-items: center;
  text-align: justify;

  &__image {
    max-width: 20rem;
    height: auto;

    img {
      width: 18rem;
    }
  }

  &__main {
    padding-left: 2rem;
    height: 100%;
    align-items: space-between;
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
}
</style>