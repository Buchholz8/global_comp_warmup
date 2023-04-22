<template>
  <div id="app">
<toast-notifactions></toast-notifactions>
<delete-button></delete-button>
<post-button></post-button>
  </div>
</template>

<script>
import ToastNotifaction from '@/components/ToastNotifaction.vue'
import DeleteButton from '@/components/DeleteButton.vue'
import PostButton from '@/components/PostButton.vue'
export default {
  name: 'App',
  components: {
ToastNotifaction,
DeleteButton,
PostButton
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
