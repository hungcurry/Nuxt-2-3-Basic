<script>
import PhotoItem from './PhotoItem.vue'
export default {
  name: 'IndexPage',
  components: {
    PhotoItem,
  },
  async asyncData(){
    return{
    }
  },
  data(){
    return {
    }
  }
};
</script>
<template>
  <div>
    <div class="card">
      <p>Card</p>
      <PhotoItem /> 
    </div>
  </div>
</template>
<style lang='scss' scoped>
  .card {
    width: 500px;
    height: 500px;
    background-color: brown;
  }
  p {
    font-size: 24px;
  }
  .muted {
    color: rgb(153, 255, 0);
  }
</style>
