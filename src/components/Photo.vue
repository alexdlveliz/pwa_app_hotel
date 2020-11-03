<template>
  <div>
    <div
      class="photo"
      v-bind:style="`background-image: url(${place.img_source}`"
    >
      <h2>{{ place.title }}</h2>
      <p>{{ place.description }}</p>
      <div class="score">
        <i class="fas fa-thumbs-up" @click="addScore"></i>
        <span>{{ place.score }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Photo",
  data() {
    return {
      rated: true,
    };
  },
  methods: {
      addScore() {
          if(this.rated)
              this.place.score++;
          this.rated = false;
      }
  },
  props: {
    place: {
      type: [Object],
      require: true,
      default: {
        img_source:
          "https://material.angular.io/assets/img/examples/shiba2.jpg",
        title: "Título de prueba",
        description: "Descripción de prueba",
        score: 0,
      },
    },
  },
};
</script>

<style>
.photo {
  height: 400px;
  width: 350px;
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin: 30px;
}

.photo h2 {
  padding: 30px 65px;
  margin-left: 15px;
  margin-right: 15px;
  background-color: var(--gradientbanner);
  backdrop-filter: blur(10px);
  font-family: var(--fontcontent);
  font-size: 18px;
  font-weight: bold;
}

.photo p {
  padding: 30px 65px;
  background-color: var(--gradientbanner);
  backdrop-filter: blur(10px);
  font-family: var(--fontcontent);
  font-size: 15px;
  font-weight: bold;
}

.photo i {
  color: rgb(76, 76, 253);
  font-size: 25px;
  margin: 0 15px;
}

.photo .score {
    display: flex;
    flex-direction: row;
    align-items: center;
    color: white;
    font-size: 25px;
}
</style>