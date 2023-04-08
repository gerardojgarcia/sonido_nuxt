<script setup>

defineProps({
    title: String,
    artist: String,
    duration: String,
    src: String,
    img: String,
    alt: String
})

function playTrack() {
    const audio = document.querySelector('.track')

    
    audio.play() 
} 

function pauseTrack() {
    const audio = document.querySelector('.track')

    
    audio.pause() 
}

</script>

<template>



<div class="music-player p-16 border-4 border-black rounded-xl" >

<div class="track-header flex space-x-16 items-center ">
    <img :src="img" :alt="alt" class="h-52 w-52 rounded-full">


    <div class="track-info  p-6   ">
        <strong class="text-3xl">{{ title }}</strong>
        <p class="track-artist text-xl">{{ artist }}</p>
        <p class="track-duration">{{ duration }}</p>
</div>
    
   
</div>
<audio class="track hidden    "  controls >
    

    <source class="track-src " :src="src" type="audio/mpeg" >

</audio>

<div class="music-controls flex flex-row">

    <AppButton title="Play" @click="playTrack()"/>
    <AppButton title="Pause" @click="pauseTrack()"/>



</div>

</div>
</template>
<style>
.music-player {
    max-height: 25rem;
    margin: 5rem;
}

</style>
