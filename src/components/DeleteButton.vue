<template>
  <div>
    <button @click="delete_func">Delete</button>
  </div>
</template>

<script>
export default {
  methods: {
    delete_func: function () {
      this.$root.$emit(`toast_notify` , `Item Deleted`);
    },
  },
};
</script>

<style scoped>
</style>