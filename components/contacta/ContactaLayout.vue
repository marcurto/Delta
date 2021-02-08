<template>
  <section class="contacta">
    <div class="contacta__image"></div>
    <div class="contacta__main">
      <h3>CONTACTA AMB NOSALTRES</h3>
      <p>Contacta amb nosaltres i estarem encantats de resoldre’t qualsevol dubte o d’atendre qualsevol consulta. </p>
      <Form/>
    </div>
  </section>
</template>

<script>
import Form from "@/components/ui/molecules/Form.vue";


export default {
  layout: "default",
  components: {
    Form
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.contacta {
  height: 100vh;
  background-color: variables.$brown-overally;
  display: grid;
  grid-template-columns: 1fr 2fr;

  &__image {
    height: 100vh;
    width: 100%;
    background-image: url("~static/img/contacta.png");
    background-repeat: no-repeat;
    background-size: cover;
  }

  &__main{
    padding: 5rem 4rem;

    p{
      margin-top: 0rem;
    }
  }
}
</style>
