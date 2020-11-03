<template>
  <div id="photos" class="text-center">
    <div class="container">
      <div class="row">
        <div class="twelve columns txt">
          <h3>Lorem, ipsum dolor.</h3>
        </div>
      </div>
      <div class="photos-container">
        <Photo class="photo" v-for="photo of photos" :key="photo.id" :place="photo"></Photo>
      </div>
    </div>
  </div>
</template>

<script>
import Photo from './Photo';

export default {
  name: "Photos",
  components:{
    Photo
  },
  data() {
    return {
      photos: [],
    };
  },
  methods: {
    async getEntries() {
      let entries = await fetch('http://localhost:8000/api/places')
        .then(res => res.json());
      this.photos = entries.data;
    }
  },
  mounted() {
    this.getEntries();
  }
};
</script>

<style scoped>
#photos {
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;
}
#photos .container {
  min-width: 80%;
  height: 80%;
}
#photos .container .row .txt h3 {
  font-family: var(--fontsubt);
  font-size: 35px;
}

#photos .container .photos-container {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: center;
}
</style>