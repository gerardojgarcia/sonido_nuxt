<script setup>

function active(){
    const trackNavItem = document.querySelector('.track-item')

    if (trackNavItem.classList.contains('.active') == true){
        trackNavItem.classList.remove('.active')
    } else {
        trackNavItem.classList.add('.active')
    }
}


</script>

<template>


    <div>
    
    <ul class=" track-list-nav flex flex-col ">
        <NuxtLink class="track-item" @click="active()" to="/adiosadiosone">Adios Adios Amor Vol. 1</NuxtLink>
        <NuxtLink class="track-item" to="/balearicone" >Balearic Vol. 1</NuxtLink>
        <NuxtLink class="track-item">Balearic Vol. 2</NuxtLink>
        <NuxtLink class="track-item"></NuxtLink>
        <NuxtLink class="track-item"></NuxtLink>

    
    </ul>
    
    
    </div>


</template>

<style scoped>

 .track-list-nav {
    max-width: 25rem;
 }

 .track-item {
    font-size: 2rem;
    background-color: #f8d6b3 ;

    margin: 1rem 0rem;
    padding: 5px;
    transition: transform 350ms;
    
 }

 .track-item:hover {
    box-shadow: 8px 10px #FF6b6b;
    border: .4rem solid black;
    transform: translateX(50px) ;

 }

 .active {
    box-shadow: 8px 10px #FF6b6b;
    border: .4rem solid black;
    transform: translateX(50px) ;

 }

</style>