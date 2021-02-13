<template>
  <div class="carouser-view">
    <carousel>
      <carousel-slide
        v-for="slide in slides"
        :key="slide"
        class="carouser-slider"
      >
        <!-- <img :src="slide" :alt="slide"> -->
        <div>
          <h4>PRESPECTIVA ÀMPLIA I GLOBAL</h4>
          <p>
            Una perspectiva àmplia i global (temàtica i geogràfica) que tingui
            en compte la interdependència i disparitat dels sistemes naturals i
            les activitats humanes que tenen incidència al delta de l’Ebre.
          </p>
        </div>
         <div>
          <h4>PRESPECTIVA ÀMPLIA I GLOBAL</h4>
          <p>
            Una perspectiva àmplia i global (temàtica i geogràfica) que tingui
            en compte la interdependència i disparitat dels sistemes naturals i
            les activitats humanes que tenen incidència al delta de l’Ebre.
          </p>
        </div>
         <div>
          <h4>PRESPECTIVA ÀMPLIA I GLOBAL</h4>
          <p>
            Una perspectiva àmplia i global (temàtica i geogràfica) que tingui
            en compte la interdependència i disparitat dels sistemes naturals i
            les activitats humanes que tenen incidència al delta de l’Ebre.
          </p>
        </div>
         <div>
          <h4>PRESPECTIVA ÀMPLIA I GLOBAL</h4>
          <p>
            Una perspectiva àmplia i global (temàtica i geogràfica) que tingui
            en compte la interdependència i disparitat dels sistemes naturals i
            les activitats humanes que tenen incidència al delta de l’Ebre.
          </p>
        </div>
      </carousel-slide>
    </carousel>
  </div>
</template>

<script>
import Carousel from "@/components/ui/atoms/Carousel.vue";

import CarouselSlide from "@/components/ui/atoms/CarouselSlide";
export default {
  data() {
    return {
      slides: ["0", "1", "2", "3", "4", "5", "6", "7"],
    };
  },
  components: {
    Carousel: Carousel,
    CarouselSlide: CarouselSlide,
  },
};
</script>

<style>
.carouser-view {
  display: flex;
  justify-content: center;
}
.carousel {
  position: relative;
  overflow: hidden;
  height: auto;
  width: 800px;
  z-index: 10;
  text-align: center;
  padding: 2rem 4rem 4rem 4rem;
}
.btn {
  padding: 5px 10px;
  background-color: rgba(0, 0, 0, 0.5);
  border: 1px solid transparent;
  margin: 5px 10px;
  color: #fff;
  height: 50px;
  width: 50px;
  position: absolute;
  margin-top: -30px;
  z-index: 2;
}
.btn:hover {
  cursor: pointer;
}
.btn:focus {
  outline: none;
}
.btn-next {
  top: 50%;
  right: 0;
}
.btn-prev {
  top: 50%;
  left: 0;
}
.carousel-slider {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  display: flex;
  flex-direction: column;
}
.carousel-slider img {
  width: 100%;
  height: 100%;
}
</style>