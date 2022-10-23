<template>
  <!--label将input包住，点击label就相当于点击input-->
  你最爱：{{x}}
  <label>
    <input name="want" type="radio" v-model="x" :value="1">
    <span>苹果</span>
  </label>
  <label>
    <input name="want" type="radio" v-model="x" :value="2">
    <span>番茄</span>
  </label>
  <label>
    <input name="want" type="radio" v-model="x" :value="3">
    <span>菠萝蜜</span>
  </label>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      x: ''
    }
  },
  components: {}
}
</script>
