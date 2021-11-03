<template>
  <div id="app">
    <List></List>
  </div>
</template>

<script>
// import axios from 'axios'
// Vue.prototype.$axios = axios
import List from './components/List.vue'
// 次にやるのはこのコンポーネントの値を下のaxiosを利用してうまくGo側に渡す方法を考える
// axiosでGo側にデータを送るのはApp.vue?それともList.vue??
export default {
  components: {
    List
  },
  // created() {
  //   this.$axios.get('http://localhost/api/')
  //   .then(response => {
  //     console.log(response)
  //   })
  // }

}
</script>

