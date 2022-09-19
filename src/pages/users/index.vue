<template>
  <Users />
</template>
<script>
import Users from './../../component/users/index.vue';
export default {
  created() {
    this.$store.dispatch('actionUsers');
  },
  components: {
    Users,
  },
};
</script>
