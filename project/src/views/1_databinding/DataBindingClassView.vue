<template>
  <div>
    <!-- 클래스 바인딩 Object - key:value (실무에서 주로 사용)-->
    <div :class="{'text-red': true, active: isActive}">클래스 바인딩</div>
    <!-- 클래스 바인딩 Array -->
    <div :class="class2">클래스 바인딩2</div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      isActive: false,
      hasError: false,
      class2: ['active', 'hasError']
    }
  },
  setup() {},
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
<style scoped>
.active {
  background-color: greenyellow;
  font-weight: bold;
}
.text-red {
  color: red;
}
</style>
