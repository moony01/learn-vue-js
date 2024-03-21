<template>
  <AppHeader 
    v-bind:appTitle="message"
    v-on:change="chageMessage">
  
  </AppHeader>
</template>

<script>
// import 컴포넌트이름 from './컴포넌트 경로'
import AppHeader from './components/AppHeader.vue'

export default {
  components: {
    // '컴포넌트이름': 컴포넌트 내용
    // 01.'app-header': AppHeader
    // 02.'AppHeader': AppHeader
    // 03.AppHeader: AppHeader
    AppHeader
  },
  data() {
    return {
      message: '앱 헤더 컴포넌트'
    }
  },
  methods: {
    // showAlert() {
    //   alert('hello');
    // },
    chageMessage() {
      this.message = '변경됨'
    }
  }
}
</script>

<style scoped>

</style>