<template>
  <!-- 문자열 바인딩 -->
  <div>
    <h1>Hello {{ userName }}</h1>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userName: 'user',
      message: 'Welcome Vue',
      arr: [],
      abj: {}
    }
  }
}
</script>

<style scoped>
.text-red {
  color: red;
}
</style>
