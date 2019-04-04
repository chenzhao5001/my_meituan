<template>
  <div>
    <ul>
      <li v-for="(item,idx) in list" :key="idx">{{item}}</li>
    </ul>
    <div class="m-geo">
      <i class="el-icon-location"/>北京市
      <nuxt-link class="changeCity" to="/aa">切换城市</nuxt-link>
      [想和 天才]
    </div>
  </div>
</template>

<script>
  import axios from 'axios'
  export default {
    name: "MyPage",
    data: function () {
      return {
        list: []
      }
    },

    async asyncData() {
      let {status,data}= await axios.get('http://127.0.0.1:3000/city/list');
      return {
        list:data
      }
    }

  }
</script>

<style lang="scss" scoped>

  /**{*/
  /*margin: 0;*/
  /*padding: 0;*/
  /*}*/

  /*li {*/
    /*list-style-type: none;*/
  /*}*/

</style>
