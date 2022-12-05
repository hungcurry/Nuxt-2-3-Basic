<script>
import axios from "axios";
export default {
  async asyncData(){
    let data = [];
    const res = await axios.get("http://www.mocky.io/v2/5cc3f5723400005d00765480");
    console.log(res.data.twzip.city);
    data = res.data.twzip.city;
    return{
      data
    }
  },
  data(){
    return{ }
  },
};
</script>
<template>
  <div>
    <h2>This is an async</h2>
    <ul v-for="(item , idx) in data" :key="item.name">
      <li>{{ item.name }}</li>
    </ul>
  </div>
</template>
<style lang='scss' scoped>
</style>

