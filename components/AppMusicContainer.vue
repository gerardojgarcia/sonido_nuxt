<script setup>

const tracks = reactive([
    {
        id:1,
        title: 'Adios Adios Amor',
        artist: 'DJ El Chante',
        duration: '47:31',
        src: '/adiosadiosamor_Vol2.mp3',
        img: '/Screenshot from 2022-06-20 01-24-53.png',
        alt: 'Cover for Adios Adios Amor'
        
    },
])


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

    <div class="music-container grid place-items-center w-3/4 m-auto rounded-sm border-black border-4">


        <div class="flex ">
            <strong class="text-5xl">Mixxes</strong>
        </div>

        <div class="music-player p-16" v-for="track in tracks" :key="track.id">

            <div class="track-header flex space-x-16">
                <img :src="track.img" :alt="track.alt">
                <div class="track-info border-4 p-6 border-black  ">
                    <strong class="text-3xl">{{ track.title }}</strong>
                    <p class="track-artist text-xl">{{ track.artist }}</p>
                    <p class="track-duration">{{ track.duration }}</p>
            </div>
                
               
            </div>
            <audio class="track hidden"  controls >
                

                <source class="track-src " :src="track.src" type="audio/mpeg" >

            </audio>

            <div class="music-controls flex flex-row">

                <AppButton title="Play" @click="playTrack()"/>
                <AppButton title="Pause" @click="pauseTrack()"/>



            </div>

        </div>


    </div>


</template>

<style scoped>

.music-container{
    box-shadow: 4px 6px #F8D6B3;
}


.track-info {
    background-color: #F8D6B3;
    min-height:;
}
</style>