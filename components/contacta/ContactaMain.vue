<template>
  <section class="contact">
    <div class="contact__section">
      <div>
        <h6>EMAILS DE CONTACTE: </h6>
        <UiList>
          <li>administracio@taulaconsens.cat</li>
          <li >direcciotecnica@taulaconsens.cat</li>
          <li>secretaria@taulaconsens.cat</li>
          <li>portaveu@taulaconsens.cat</li>
          <li>presidencia@taulaconsens.cat</li>
        </UiList>
      </div>
       <div>
         <h6>TELÈFONS DE CONTACTE: </h6>
        <UiList>
          <li>+34 977 48 06 80</li>
          <li >+34 652 061 315</li>
        </UiList>
      </div>
    </div>
    <hr></hr>
    <div class="contact__section">
      <div class="contact__share">
      <h6>COMPARTEIX: </h6>
      <div>
        <img src="~static/img/008-instagram-1.png" />
        <img src="~static/img/006-twitter-1.png" />
        <img src="~static/img/007-linkedin-1.png" />
      </div>
      </div>
    </div>
  </section>
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

.contact {
  height: 30vh;
  width: 100%;
  display: flex;
  align-items: center;

  &__section {
    display: flex;
    width: 100%;
    height: 100%;
    justify-content: space-around;
    align-items: flex-start;
    padding-top: 4rem;
  }

  &__share {
    display: flex;
    height: 100%;
    width: 100%;
    justify-content: flex-start;
    align-items: flex-start;
    flex-direction: column;
    padding: 4rem;

    img{
      width: 30px;
    }
  }

  hr {
    height: 20vh;
  }

  h6 {
    font-weight: 400;
    margin-bottom: 1rem;
    color: variables.$black;
  }

  li {
    letter-spacing: 0.8px;
    margin-bottom: 0.2rem;
    font-size: variables.$text-s;
    font-family: variables.$font-damily-alternative;
  }
}
</style>
