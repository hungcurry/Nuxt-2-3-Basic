<script>
export default {
  name: 'window',
  async asyncData(){
    // node 裡面沒有window / document 會報錯
    // console.log(window);
    console.log('process' ,process.client); // false

    return{
    }
  },
  data(){
    return {
    }
  },
  mounted(){
    console.log('process' ,process.client); // true
    console.log(window);
  }
};
</script>
<template>
  <div>
  </div>
</template>
<style lang="scss" scoped>
</style>
