<template>
  <!--label将input包住，点击label就相当于点击input-->
  你最爱：{{x}}
  <select v-model="x">
<!--    <option value>-</option>-->
<!--    <option :value="1">苹果</option>-->
<!--    <option :value="2">香蕉</option>-->
<!--    <option :value="3">橘子</option>-->

<!--    用v-for渲染-->
    <option v-for="item in array" :value="item.value" :key="item.value">{{item.text}}</option>
  </select>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      // 选择框中的数据来自数组（后台）
      array: [
        {text: '苹果', value: 1},
        {text: '香蕉', value: 2},
        {text: '橘子', value: 3},
      ],
      x: []
    }
  },
  components: {}
}
</script>
