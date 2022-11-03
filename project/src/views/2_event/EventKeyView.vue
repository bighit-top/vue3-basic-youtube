<template>
  <div>
    <!-- keyup 이벤트 기본: enter key 13번 세팅해서 처리 -->
    <!-- <input type="search" name="" id="" @keyup="checkEnter($event)" v-model="searchText" /> -->
    <!-- keyup 이벤트 vue 제공 기능: 주요 key 제공(enter, space, esc, tab, up, down...) -->
    <input
      type="search"
      name=""
      id=""
      @keyup.enter="checkEnter($event)"
      v-model="searchText" />
    <button @click="doSearch">조회</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      searchText: ''
    }
  },
  setup() {},
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    doSearch() {
      console.log(this.searchText)
    },
    checkEnter(event) {
      if (event.keyCode === 13) {
        this.doSearch()
      }
    }
  }
}
</script>
