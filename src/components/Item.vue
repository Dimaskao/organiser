<template>
  <div @dblclick="goTo(item.path)" class="col">
    <div class="p-3">
      {{item.title}}
    </div>
  </div>
</template>

<script>
  export default {
    props: {
      item: {
        type: Object,
        required: true
      }
    },
    methods: {
      goTo(path) {
        open(path)
      }
    }
  }
</script>

<style scoped>
</style>