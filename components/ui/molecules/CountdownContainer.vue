<template>
  <section class="inicio">
    <div class="inicio__item">
    <h3>El Delta de l’Ebre pot desaparèixer en...</h3>
    </div>
        <div class="inicio__item">
    <Countdown date="2021-07-17 08:15:00"/>
        </div>
        <div class="inicio__item">

    <Button />
        </div>
  </section>
</template>

<script>
import Countdown from "@/components/ui/atoms/Countdown.vue";
import Button from "@/components/ui/atoms/Button.vue";

export default {
 components: {
   Countdown,
   Button
 }
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.inicio{
  height: 100vh;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;

  &__item{
    height: 100%;
    width: 100%;
      display: flex;
    align-items: center;
    justify-content: center;

  }

  @media (max-width: 800px) {
      h3{
        font-size: variables.$subtitle;
      }
  }
  @media (max-width: 600px) {
      h3{
        text-align: center;
        padding: 0rem 2.5rem;
        margin-top: 2.5rem;
      }
  }

}
</style>