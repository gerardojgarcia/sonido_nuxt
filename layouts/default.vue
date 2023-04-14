<template>
<div>
  <AppHeader/>


  <div class="flex flex-col md:flex-row justify-around py-16 m-auto">
    <AppTrackList class="pb-16"/>
    <slot class="md:w-1/2" />
  </div>
</div>
</template>

<script setup>

</script>

<style scoped>


</style>
