<script setup>

// node 裡面沒有window / document 會報錯
// console.log(window);

console.log('process' ,process.client);
// 瀏覽器 會寫 true  ==>  代表 是在 client 瀏覽器上
// 終端機 會寫 false ==>  代表 不在 client 瀏覽器上
if(process.client){
  console.log(window);
}

// 必須放在 onMounted 生命週期取得
// onMounted(() => {
//   console.log(window);
// });

</script>
<template>
  <div></div>
</template>
<style lang='scss' scoped>
</style>
