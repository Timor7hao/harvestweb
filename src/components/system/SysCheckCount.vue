<template>
  <div id="sysCheckCount">
    <div class="all-title">
      <p class="main-font">
        <span>查询条件</span>
        <el-button v-if="$type === '0'" type="primary" size="small" @click="searchHarvest()">查询</el-button>
        <el-button v-else-if="$type === '2'" type="warning" size="small" @click="searchHarvest()">查询</el-button>
        <el-button type="danger" size="small" style="margin-right: 15px;" @click="resetForm()">重置</el-button>
      </p>
    </div>
    <div>
      <advance-search></advance-search>
      <check-result></check-result>
    </div>
  </div>
</template>

<script>
  import AdvanceSearch from '@/components/table/TabAdvanceSearch'
  import CheckResult from '@/components/form/formCheckResult'
  import myapi from '@/api/myapi.js'
  export default {
    name:'sysCheckCount',
    components:{
      AdvanceSearch,
      CheckResult
    },
    data () {
      return {
        
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
