<template>
  <div class="images-logos">
    <img
      src="~static/img/deltebre.png"
      alt=""
      class="description__images__item"
    />
    <img
      src="~static/img/santjaume.png"
      alt=""
      class="description__images__item"
    />
    <img
      src="~static/img/rapita.png"
      alt=""
      class="description__images__item"
    />
    <img
      src="~static/img/amposta.png"
      alt=""
      class="description__images__item"
    />
    <img
      src="~static/img/camarles.png"
      alt=""
      class="description__images__item"
    />
    <img
      src="~static/img/ampolla.png"
      alt=""
      class="description__images__item"
    />
    <img src="~static/img/aldea.png" alt="" class="description__images__item" />
    <img
      src="~static/img/comunitat.png"
      alt=""
      class="description__images__item"
    />
    <img
      src="~static/img/comunitat_esquerra.png"
      alt=""
      class="description__images__item"
    />
  </div>
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

.images-logos {
  width: 100%;
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;

  img {
    width: auto;
    height: 100px;
    display: block;
  }

  @media (max-width: 800px) {
    img {
      height: 80px;
    }
  }
  @media (max-width: 500px) {
    justify-content: center;
    img {
      height: 70px;
      margin: 0.3rem;
    }
  }
}
</style>

    
    
   