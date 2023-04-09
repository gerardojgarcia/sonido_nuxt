<script setup>

defineProps({
    title: String,
    action: String,

}) 




</script>

<template>
    <div class="m-4">
        <button  id="app-btn" class="rounded-sm border-black border-4 p-3 duration-150 ">{{ title }} </button>
    </div>




</template>
<style scoped>

#app-btn {
    background-color: #F8D6B3;
}

#app-btn:hover {
    box-shadow: 4px 6px black;
    transform: translateX(-5px) translateY(-5px);
    
} 



</style>
