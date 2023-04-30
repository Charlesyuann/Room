<template>
  <div class="home">
<label>搜尋：
    <input type="text" v-model="inputText" />
</label>
<pre>即時顯示輸入內容：{{ inputText }}</pre>
<!-- {{over}} -->
    <img alt="Vue logo" src="../assets/OIP.jpg">
    <HelloWorld msg="Welcome my Project"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  data() {
  return {
    inputText: "",
    num: 50
  };
},
// computed:{
//   over(){
//     return this.num *2
//   }
// }
}
</script>
