<template>
  <div id="grid">
    <appImage v-for="(image, index) in randomImageGrid" :image="image" :key="index"></appImage>
  </div>
</template>

<script>
import _ from 'lodash'
import {ImagesMixin} from './ImagesMixin.js';
import Image from './Image.vue';

export default {
  data () {
    return {
      // msg: 'Welcome to Your Vue.js App'
    }
  },
  computed: {
    randomImageGrid(){
      return _.shuffle(this.images).slice(0,20);
    }
  },
  mixins: [ImagesMixin],
  components: {
    appImage: Image
  }
}
</script>

<style lang="scss">
body {
  background-color: #ddd;
}
#grid {
  margin: 0 auto;padding: 0;
  width: 800px;
}
</style>
