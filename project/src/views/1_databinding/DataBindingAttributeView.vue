<template>
  <div>
    <!-- 단방향 HTML Attribute 바인딩 - 기본 -->
    <div>
      <input type="text" name="" id="" v-bind:value="userId" readonly />
    </div>
    <!-- 단방향 HTML Attribute 바인딩 - 생략 -->
    <div>
      <input type="text" name="" id="" :value="userId" readonly />
    </div>
    <!-- HTML Attribute 이미지 바인딩 -->
    <div>
      <img :src="imgSrc" alt="" style="width:100px; height:auto;" />
    </div>
    <!-- HTML Attribute 필수값 바인딩 -->
    <div>
      <input type="search" name="" id="" v-model="txt1" />
      <button :disabled="txt1 === ''">조회</button>
    </div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userId: 'user',
      imgSrc: 'https://upload.wikimedia.org/wikipedia/commons/f/f1/Vue.png',
      txt1: ''
    }
  },
  setup() {},
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
