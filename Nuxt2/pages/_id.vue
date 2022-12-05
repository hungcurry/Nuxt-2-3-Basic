<script>
export default {
  name: 'id',
  async asyncData(context){
    // console.log(context);
    const NuxtPath = context.route.path;
    const NuxtId = context.params.id;
    return{
      NuxtPath , NuxtId
    }
  },
  data(){
    return {
      path : this.$route.path,
      id : this.$route.params.id,
    }
  },
  mounted(){
    console.log("route" , this.$route);
    console.log("router" ,this.$router);
  }
}
</script>
<template>
  <div>
  <h1>動態網址</h1>
    <p>Nuxt2 asyncData => <span class="tags">{{ NuxtPath }}</span></p>
    <p>Nuxt2 asyncData => <span class="tags">{{ NuxtId }}</span></p>

    <p>Vue2 => <span class="tags">{{ path }}</span></p>
    <p>Vue2 => <span class="tags">{{ id }}</span></p>
  </div>
</template>
<style lang='scss' scoped>
.tags {
  color: red;
}
</style>
