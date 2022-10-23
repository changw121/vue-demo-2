<template>
  <textarea v-model="message" placeholder="edit me"/>
  <p>Message is: {{ message }}</p>
  <p><button @click="message = 'changw'">set message to changw</button></p>
</template>

<script>

export default {
  name: 'App',
  data() {
    return{
      message: 'hi'
    }
  },
  components: {}
}
</script>
