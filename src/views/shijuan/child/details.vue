<template>
    <div>
       {{$route.params.id}}
    </div>
</template>

<script>

import { mapMutations } from 'vuex';

export default {
  name: 'details',
  methods: {
    ...mapMutations(['addKeepAlive']),
  },
  created() {
    this.addKeepAlive('daitishen');
  },
};
</script>

<style scoped>

</style>
