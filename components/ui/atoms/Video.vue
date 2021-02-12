<template>
        <div class="video" v-if="video">
            <iframe v-bind:src="url" ></iframe>
        </div>

</template>



<script>
    export default {
      created() {
        //   if (this.$route.params.video === undefined) {
        //       this.$router.push({name: 'youtube-dash'});
        //   }

          this.videoId = this.$route.params.id;
          this.url = `https://www.youtube.com/embed/${this.videoID}`;
          this.video = this.$route.params.video;
      },

      data() {
          return {
              videoId: null,
              video: null,
              url: null
          }
      }
    }
</script>