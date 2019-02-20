<template>
  <div id="testResume">
    <div class="main-content">
      <user-info></user-info>
      <div class="all-title">
        <p class="main-font">
            <span>个人成果</span>
        </p>
      </div>
      <img src="@/assets/testHarvest.jpg">
    </div>
  </div>
</template>

<script>
  import UserInfo from '@/components/system/SysUserinfo'
  import myapi from '@/api/myapi.js'
  export default {
    name: 'testResume',
    components:{
      UserInfo
    },
    data () {
      return {
        
      }
    },
    methods: {
    }
  }
</script>

<style scoped>
.main-content {
  margin: 80px 500px;
}
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
