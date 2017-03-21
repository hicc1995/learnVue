<template>
<el-row>
  <el-col :span="6"><login class="grid-content bg-purple"></login></el-col>
  <el-col :span="12"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
</el-row>
</template>
<script>
var login = require('../login.vue')

module.exports = {
  components: {
    'login': login
  }
}
</script>