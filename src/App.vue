<template>
<head>
  <link rel="shortcut icon" href="https://i.imgur.com/9gZF4K9.png" type="image/x-icon">
</head>
<homepage />
</template>

<script>
import Homepage from './views/Homepage.vue'

export default {
  name: 'App',
  components: {
    Homepage
  }
}
</script>

<style scoped> 
.main-content{
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>
