<template>
  <div>
    <h2 @mouseover="incrementCount">Hovered {{ count }} times</h2>
  </div>
</template>

<script setup>
  import { ref } from 'vue';

  const count = ref(0)

  const incrementCount = () => {
    count.value++
  }

</script>

<style lang="scss" scoped>

</style>