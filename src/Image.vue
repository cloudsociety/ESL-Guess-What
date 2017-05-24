<template>
  <div class="image" @click="visible = !visible">
    <img :src="image" alt="" class="image__face" :class="{'image__face--hidden':!visible}">
  </div>
</template>

<script>
  export default {
    data: function() {
      return {
        visible: true
      }
    },
    props: ['image']
  }
</script>

<style lang="scss">
.image {
  width: 150px; height: 150px;
  background: #fff url('assets/bg-img.png') center center no-repeat;
  background-size: cover;
  border-radius: 10px;
  box-shadow: 0 0 5px #999;
  display: inline-block;
  // float: left;
  margin: 5px;padding: 0;
  overflow: hidden;

  &__face {
    margin: 0;padding: 0;
    width: 150px; height: 150px;
    object-fit:cover;
    &--hidden {
      visibility: hidden;
    }
  }
}
</style>
