<template>
  <div id="formCheckResult">
    <div class="all-title">
      <p class="main-font">
        <span>查询结果</span>
      </p>
    </div>
    <img src="@/assets/testHarvest.jpg">
  </div>
</template>

<script>
  import myapi from '@/api/myapi.js'
  export default {
    name: 'formCheckResult',
    data () {
      return {

      }
    },
    methods: {
        
    }
  }
</script>

<style scoped>
.all-title {
  height: 40px;
  border-bottom: 1px dashed #DCDFE6;
}
.main-font {
  font-size: 17px;
  color: #000;
  font-family: Hiragino Sans GB;
}
.el-button{
  float: right;
}
</style>
