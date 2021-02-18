<template>
  <div class="countdown">
    <div class="countdown__item">
      <span>{{years}}</span>
      <p>ANYS</p>
    </div>
    <div class="countdown__item">
      <span>{{months}}</span>
      <p>MESOS</p>
    </div>
    <div class="countdown__item">
      <span>{{days}}</span>
      <p>DIES</p>
    </div>
    <div class="countdown__item">
      <span>{{hours}}</span>
      <p>HORES</p>
    </div>
    <div class="countdown__item">
      <span>{{minutes}}</span>
      <p>MINUTS</p>
    </div>
    <div class="countdown__item">
      <span>{{seconds}}</span>
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
    date: {
      type: String
    }
  },
  
  data() {
    return {
      now: Math.trunc((new Date()).getTime() / 1000)
    }
  },
  created: function(){
    setInterval(() => {
        this.$data.now = Math.trunc((new Date()).getTime() / 1000);
    }, 1000);
  },
  methods: {
    two_digits(value){
      if (value < 0) {
        return '00';
      }
      if (value.toString().length <= 1) {
        return `0${value}`;
      }
      return value;
    },
  },
  computed: {
    
    dateInMilliseconds() {
      return Math.trunc(Date.parse(this.$props.date) / 1000)
    },
    seconds() {
      return this.two_digits((this.dateInMilliseconds - this.$data.now) % 60);
    },
    minutes() {
      return this.two_digits(Math.trunc((this.dateInMilliseconds - this.$data.now) / 60) % 60);
    },
    hours() {
      return this.two_digits(Math.trunc((this.dateInMilliseconds - this.$data.now) / 60 / 60) % 24);
    },
    days() {
      return this.two_digits(Math.trunc((this.dateInMilliseconds - this.$data.now) / 60 / 60 / 24) % 30);
    },
    months() {
      return this.two_digits(Math.trunc((this.dateInMilliseconds - this.$data.now) / 60 / 60 / 24 / 30) % 12);
    },
    years() {
      return this.two_digits(Math.trunc((this.dateInMilliseconds - this.$data.now) / 60 / 60 / 24 / 365));
    }
  }
};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";

.countdown {
  font-family: "Roboto Slab", serif;
  font-size: 6rem;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;

  &__item {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-width: auto;
    width: 10rem;
    margin: 0.7rem;
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

  @media (max-width: 1300px) {
    &__item {
      width: 8rem;
    }
    span {
      font-size: variables.$title-l;
    }
  }

  @media (max-width: 1100px) {
    &__item {
      width: 7rem;
    }
    span {
      font-size: variables.$title-m;
    }
  }

  @media (max-width: 900px) {
  
  }

  @media (max-width: 500px) {
    width: 100%;

    &__item{

      padding: 0.2rem;
    }
     span {
      font-size: variables.$title-s;
    }
    p {
      font-size: variables.$item;
    }
  }
}
</style>