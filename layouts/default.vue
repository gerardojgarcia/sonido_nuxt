<template>
<div>
  <AppHeader/>


  <div class="flex flex-col md:flex-row justify-around  m-auto">
    <AppTrackList/>
    <slot class="md:w-1/2" />
  </div>
</div>
</template>

<script setup>

</script>

<style scoped>


</style>