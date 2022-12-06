<template lang="pug">
h1 吉他社首頁
input(type="button" value="回社團首頁" @click="goto('/guitar')")
input(type="button" value="活動公告" @click="goto('/guitar/events')")
input(type="button" value="教學內容" @click="goto('/guitar/teach')")
</template>

<script setup>
import { useRouter } from 'vue-router'
// router是可以操作路由的變數
// route是取得目前路由資訊的變數
const router = useRouter()
// const route = useRoute()
// console.log(route)
const goto = (path) => {
  router.push(path)
}
</script>
<!-- <script>
export default {
  methods: {
    goto (path) {
      this.$router.push(path)
    }
  }
}
</script> -->
