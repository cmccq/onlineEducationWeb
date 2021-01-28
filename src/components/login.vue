<template>
  <div class="divBg">
      <div class="loginBox">
        <el-form
          :model="myForm"
          :label-position="labelPosition"
          :label-width="25+'%'"
        >
          <el-form-item prop="username" label="账号:">
            <el-input v-model="myForm.username" style="width: 80%;"></el-input>
          </el-form-item>
          <el-form-item prop="password" label="密码:">
            <el-input v-model="myForm.password" show-password style="width: 80%"></el-input>
          </el-form-item>
          <el-form-item prop="verifyCode" label="验证码:">
            <el-input v-model="myForm.verifyCode" style="width: 80%"></el-input>
          </el-form-item>
          <el-form-item>
            <div style="padding-left:15%;">
                <el-button type="primary">注册</el-button>
                <el-button type="primary">登录</el-button>
                <span><a href="#">忘记密码?</a></span>
            </div>
          </el-form-item>
        </el-form>
      </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      // 表单标题位置
      labelPosition: 'right',
      myForm: {
        username: '',
        password: '',
        verifyCode: ''
      }
    }
  },
  methods: {}
}
</script>

<style>
.loginBox {
  width: 30%;
  height: 40vh;
  background: rgba(204, 86, 86, 0.03);
  margin-left: 35%;
  padding-top: 10vh;
  margin-top: 10%;
}
.divBg{
  width: 100%;
  height: 100vh;
  display: inline-block;
}
</style>
