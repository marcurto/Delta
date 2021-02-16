
<template>
  <div class="carousel">
    <VueSlickCarousel
      :arrows="true"
      :dots="true"
      v-bind="settings"
      class="carousel-o"
    >
      <div class="carousel__item">
        <div>
          <p>UNA PRESPECTIVA ÀMPLIA I GLOBAL</p>
          <p>
            Temàtica i geogràfica que tingui en compte la interdependència i
            disparitat dels sistemes naturals i les activitats humanes que tenen
            incidència al delta de l’Ebre
          </p>
        </div>
      </div>
      <div class="carousel__item">
        <p>UNA PRESPECTIVA A LLARG TERMINI</p>
        <p>
          Que tingui en compte el principi de cautela i les necessitats de les
          generacions actuals i futures
        </p>
      </div>
      <div class="carousel__item">
        <p>UNA GESTIÓ MODULADA</p>
        <p>
          En un procés gradual que faciliti les adaptacions segons sorgeixin
          problemes i evolucionin els coneixements. Això exigeix ​​una sòlida
          base científica relativa a l'evolució de les zones costaneres
        </p>
      </div>
      <div class="carousel__item">
        <p>LES CARACTERÍSTIQUES LOCALS I LA DIVERSITAT</p>
        <p>
          Dels ambients deltaics, de manera que pugui respondre a les seves
          necessitats pràctiques amb solucions específiques i mesures flexibles
        </p>
      </div>
      <div class="carousel__item">
        <p>UN TREBALL EN SINTONIA AMB ELS PROCESOS NATURALS</p>
        <p>
          Que respecte la capacitat de càrrega dels ecosistemes, amb la qual
          cosa les activitats humanes seran més respectuoses amb el medi
          ambient, més responsables socialment i racionals, des del punt de
          vista econòmic, a llarg termini
        </p>
      </div>
      <div class="carousel__item">
        <p>LA PARTICIPACIÓ DE TOTES LES PARTS INTERESSADES</p>
        <p>
          en el procés de gestió, per exemple, mitjançant acords i segons el
          principi de la responsabilitat compartida
        </p>
      </div>
      <div class="carousel__item">
        <p>EL SUPORT I LA PARTICIPACIÓ L'ADMINISTRACIÓ</p>
        <p>
          Competent a escala nacional, regional i local, entre les quals
          convindrà establir o mantenir els vincles adequats per millorar la
          coordinació de les diferents polítiques existents.
        </p>
      </div>
      <div class="carousel__item">
        <p>LA COMBINACIÓ D'INTRUMENTS</p>
        <p>
          Destinats a facilitar la coherència entre els objectius de la política
          sectorial i entre l'ordenació i la gestió.
        </p>
      </div>
    </VueSlickCarousel>
  </div>
</template>
<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";
export default {
  components: {
    VueSlickCarousel,
  },
  name: "slide",
  data() {
    return {
      settings: {
        dots: true,
        infinite: false,
        speed: 500,
        slidesToShow: 4,
        slidesToScroll: 4,
        initialSlide: 0,
        responsive: [
          {
            breakpoint: 1024,
            settings: {
              slidesToShow: 3,
              slidesToScroll: 3,
              infinite: true,
              dots: true,
            },
          },
          {
            breakpoint: 600,
            settings: {
              slidesToShow: 2,
              slidesToScroll: 2,
              initialSlide: 2,
            },
          },
          {
            breakpoint: 480,
            settings: {
              slidesToShow: 1,
              slidesToScroll: 1,
            },
          },
        ],
      },
    };
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.carousel {
  height: 100%;
  
  &__item {
    background-color: rgb(250, 250, 250, 0.3);
    display: flex !important;
    flex-direction: column;
    padding: 1rem;
    text-align: center;
    align-items: center;
    height: 350px;
    justify-content: flex-start;
    width: 99% !important;

    p {
      margin-top: 0px;
    }

    @media (max-width: 800px) {
      p {
        margin: 0rem;
        font-size: variables.$text-s;
      }
      &__item {
        height: 100%;
        width: 95% !important;
      }
    }
  }
}
</style>


