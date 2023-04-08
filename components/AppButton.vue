<script setup>

defineProps({
    title: String,
    action: String,

}) 

function play() {
    const audio = document.querySelector('.track')
    this.audio.play
}


</script>

<template>
    <div class="m-4">
        <button :@click="action" id="app-btn" class="rounded-sm border-black border-4 p-3 duration-150 ">{{ title }} </button>
    </div>




</template>
<style scoped>

#app-btn {
    background-color: #F8D6B3;
}

#app-btn:hover {
    box-shadow: 4px 6px black;
    
} 



</style>
