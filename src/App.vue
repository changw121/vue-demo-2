<template>
  <!--  @submit.prevent监听submit事件并阻止默认动作-->
  登录
  <form @submit.prevent="onSubmit">
    <label>
      <span>用户名</span>
      <input type="text" v-model="user.username">
    </label>
    <label>
      <span>密码</span>
      <input type="password" v-model="user.password">
    </label>
    <button type="submit">注册</button>
  </form>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      user: {
        username: '',
        password: ''
      }
    }
  },
  methods: {
    onSubmit() {
      console.log(this.user)
    }
  },
  components: {}
}
</script>
