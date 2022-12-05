<script>
// import Tutorial from "../components/Tutorial.vue";
import Card from '../components/Card/index.vue'
export default {
  name: 'IndexPage',
  components: {
    Card,
  },
  asyncData(){
    const name = "curry";
    return{
      name,
    }
  },
  data(){
    return{
      name: "",
    }
  },
  methods:{
    handClick(){
      this.name = "白爛貓"
    }
  }
};
</script>
<template>
  <div>
    <p>{{ name }}</p>
    <button @click="handClick">點我</button>
    <Card />
  </div>
</template>
<style lang='scss' scoped>
</style>


