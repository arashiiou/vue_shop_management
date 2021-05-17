<template>
  <div>
    <p>Home 元件</p>
    <el-button @click="logout" type="info">登出</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    logout () {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style scoped>

</style>
