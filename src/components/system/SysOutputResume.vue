<template>
  <div id="sysOutputResume">
    <div class="all-title">
      <p class="main-font">
        <span>个人信息</span>
        <el-button type="primary" size="small" @click="generateResume()">生成简历</el-button>
      </p>
    </div>
    <user-info></user-info>
    <check-count></check-count>
  </div>
</template>

<script>
  import CheckCount from '@/components/system/SysCheckCount'
  import UserInfo from '@/components/system/SysUserinfo'
  import myapi from '@/api/myapi.js'
  export default {
    name:'sysOutputResume',
    components:{
      CheckCount,
      UserInfo
    },
    data () {
      return {
        
      }
    },
    methods: {
      generateResume () {
        this.$router.push({ 
					name: 'TestResume'
				})                                                                                                                                                                                                                                                                                                                                                                                                                                                       
      }
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
