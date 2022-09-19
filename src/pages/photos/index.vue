<template>
  <Photos />
</template>
<script>
import Photos from './../../component/photos/index.vue';
export default {
  created() {
    this.$store.dispatch('actionPhotos', this.albumId);
  },
  components: {
    Photos,
  },
  computed: {
    albumId() {
      return this.$route.params.albumId;
    },
  },
};
</script>
