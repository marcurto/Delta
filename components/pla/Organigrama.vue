<template>
  <div class="organigrama">
    <h4>RESUM MESURES PROPOSADES</h4>
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
  padding: 1rem 0rem 4rem 2rem;
  img{
    width: 80%;
  }
  h4{
    margin-bottom: 2rem;
  }

   @media (max-width: 700px) {
    padding: 0rem;
margin-bottom: 2rem;
   
   }
}
</style>