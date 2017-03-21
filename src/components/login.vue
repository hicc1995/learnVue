<template>
<el-form ref="form" :model="form" label-width="80px">
  <el-form-item label="活动名称">
    <el-input v-model="form.name"></el-input>
  </el-form-item>
  <el-form-item label="密码">
    <el-input v-model="form.pw"></el-input>
  </el-form-item>
  <el-form-item label="特殊资源">
    <el-radio-group v-model="form.resource">
      <el-radio label="线上品牌商赞助"></el-radio>
      <el-radio label="线下场地免费"></el-radio>
    </el-radio-group>
  </el-form-item>
  <el-form-item>
    <el-button type="primary" @click="onSubmit">点击登录</el-button>
    <el-button>取消</el-button>
  </el-form-item>
</el-form>
</template>
<script>
  export default {
    data() {
      form: {
            name: '',
            resource: '',
            pw: ''
          }
      return {
        form
      }
    },
    methods: {
      onSubmit() {
        console.log(this.form.name);
      }
    },
    watch: {
      form.name: function(old) {
        console.log(old)
      }
    }
  }
</script>