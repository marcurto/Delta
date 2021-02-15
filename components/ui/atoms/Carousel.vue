
<template>
  <div>
    <VueSlickCarousel :arrows="true" :dots="true" v-bind="settings">
      <img
        class="d-block w-100"
        src="~static/img/008-instagram-1.png"
        alt="First slide"
      />
      <img
        class="d-block w-100"
        src="~static/img/008-instagram-1.png"
        alt="Second slide"
      />
      <img
        class="d-block w-100"
        src="~static/img/008-instagram-1.png"
        alt="Third slide"
      />
       <img
        class="d-block w-100"
        src="~static/img/008-instagram-1.png"
        alt="Third slide"
      />
       <img
        class="d-block w-100"
        src="~static/img/008-instagram-1.png"
        alt="Third slide"
      />
       <img
        class="d-block w-100"
        src="~static/img/008-instagram-1.png"
        alt="Third slide"
      />
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
  "dots": true,
  "infinite": false,
  "speed": 500,
  "slidesToShow": 4,
  "slidesToScroll": 4,
  "initialSlide": 0,
  "responsive": [
    {
      "breakpoint": 1024,
      "settings": {
        "slidesToShow": 3,
        "slidesToScroll": 3,
        "infinite": true,
        "dots": true
      }
    },
    {
      "breakpoint": 600,
      "settings": {
        "slidesToShow": 2,
        "slidesToScroll": 2,
        "initialSlide": 2
      }
    },
    {
      "breakpoint": 480,
      "settings": {
        "slidesToShow": 1,
        "slidesToScroll": 1
      }
    }
  ]
},
    };
  },
};
</script>


