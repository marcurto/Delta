<template>
  <div class="countdown">
    <div class="countdown__item">
      <span>25</span>
      <p>ANYS</p>
    </div>
    <div class="countdown__item">
      <span>12</span>
      <p>MESOS</p>
    </div>
    <div class="countdown__item">
      <span>23</span>
      <p>DIES</p>
    </div>
    <div class="countdown__item">
      <span>23</span>
      <p>HORES</p>
    </div>
    <div class="countdown__item">
      <span>12</span>
      <p>MINUTS</p>
    </div>
    <div class="countdown__item">
      <span>47</span>
      <p>SEGONS</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    tag: {
      type: String,
      default: "Glòria",
    },
    theme: {
      type: String,
      default: null,
      validator(value) {
        const themes = ["pla", "delta", "banner"];
        return themes.includes(value);
      },
    },
  },
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";

.countdown {
  font-family: "Roboto Slab", serif;
  font-size: 6rem;
  display: flex;

  &__item {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-width: auto;
    width: 10rem;
    margin: 0 0.7rem;
    background-color: rgb(250, 250, 250, 0.3);
    color: rgb(41, 38, 38);
    padding: 0.7rem 0.5rem;
  }
  span {
    font-family: variables.$font-family-titles;
    font-size: variables.$title;
    margin: 0 1rem;
    font-weight: 500;
    color: rgb(41, 38, 38);
  }

  p {
    font-size: variables.$subtitle;
    font-family: variables.$font-family;
    font-weight: 400;
  }
}
</style>