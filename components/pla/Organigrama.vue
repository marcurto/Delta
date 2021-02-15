<template>
  <div class="organigrama">
    <h3>RESUM MESURES PROPOSADES</h3>
    <img src="~static/img/organigrama.png" />
  </div>
</template>

<script>
export default {};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.organigrama {
  display: flex;
  flex-direction: column;
  width: 100%;
  justify-content: center;
  align-items: center;
  padding: 1rem 2rem 4rem 2rem;
  img{
    width: 80%;
  }
  h3{
    margin-bottom: 2rem;
  }
}
</style>