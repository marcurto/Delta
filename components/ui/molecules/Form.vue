<template>
  <form class="form">
    <div class="form__item">
      <label name="name">Correu electrònic:</label>
      <input type="email" name="name" placeholder="" />
    </div>
    <div class="form__item">
      <label name="subject">Assumpte:</label>
      <input type="email" name="subject" placeholder="" />
    </div>

    <div class="form__item">
      <label name="email">Missatge:</label>
      <textarea name="email" placeholder="" ></textarea>
    </div>
  </form>
</template>

<script>
export default {};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.form {
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: column;

  &__item{
    display: flex;
    flex-direction: column;
    margin-bottom: 3rem;

    input, 
    textarea {
      background-color: transparent;
      border: none;
      border-bottom: 2px solid variables.$black;
      max-height: 80px;

      &:focus{
        height: 300px;
      }
    }

    label{
      font-size: variables.$text;
      font-weight: 300;
    }
  }
}
</style>