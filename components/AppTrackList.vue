<script setup>





</script>

<template>


    <div class="md:w-1/4">
    
    <ul class=" track-list-nav overflow-x-auto md:overflow-y-auto flex md:flex-col space-x-8 md:space-x-0 md:p-8">
        <NuxtLink class="track-item text-lg md:text-4xl " to="/adiosadiosone"  >Adios Adios Amor Vol. 1</NuxtLink>
        <NuxtLink class="track-item text-lg md:text-4xl"  to="/adiosadiostwo" >Adios Adios Amor Vol. 2</NuxtLink>
        <NuxtLink class="track-item text-lg md:text-4xl" to="/adiosadiosthree" >Adios Adios Amor Vol. 3</NuxtLink>
        <NuxtLink class="track-item text-lg md:text-4xl" to="/balearicone"  >Balearic Vol. 1</NuxtLink>
        <NuxtLink class="track-item text-lg md:text-4xl" to="/balearictwo"  >Balearic Vol. 2</NuxtLink>
        <NuxtLink class="track-item text-lg md:text-4xl" to="/balearicthree"  >Balearic Vol. 3</NuxtLink>
        <NuxtLink class="track-item text-lg md:text-4xl" >Balearic Vol. 4</NuxtLink>
        <NuxtLink class="track-item text-lg md:text-4xl" >Japanese City Pop Vol. 1</NuxtLink>
        <NuxtLink class="track-item text-lg md:text-4xl" >Turkish Female Singers Vol. 1</NuxtLink>

    
    </ul>
    
    
    </div>


</template>

<style scoped>

 .track-list-nav {
    max-width: 35rem;
    max-height: 50vh;
 }

 .track-item {
    
    background-color: #f8d6b3 ;

    margin: 1rem 0rem;
    padding: 5px;
    transition: transform 350ms;
    
 }

 .track-item:hover {
    box-shadow: 5px 10px #FF6b6b;
    border: .4rem solid black;
    transform: translateX(15px)  ;
    transition: all 500ms;

 }

 .router-link-active {
    box-shadow: 8px 10px #FF6b6b;
    border: .4rem solid black;
    transform: translateX(15px) ;

 }

</style>