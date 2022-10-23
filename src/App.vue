<template>
<!--label将input包住，点击label就相当于点击input-->
  <label for="checkbox">
    <input type="checkbox" v-model="x">
    <span>x: {{ x }}</span>
  </label>
</template>

<script>

export default {
  name: 'App',
  data() {
    return{
      x: true
    }
  },
  components: {}
}
</script>
