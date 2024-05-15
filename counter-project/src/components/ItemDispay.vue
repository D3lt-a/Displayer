<template>
  <div>    
    <h3>{{ item.name }}</h3>
    <p>Contribution: {{ item.price }}</p>
  </div>
</template>

<script>
export default {
  props: {
    item: {
      type: Object,
      required: true
    }
  }
}
</script>

<style>
/* Your styles */
</style>
  