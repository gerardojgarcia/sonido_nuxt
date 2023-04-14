




<template>

  
  <div>
    <NuxtLayout>

      <NuxtPage/>
      </NuxtLayout>

  </div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Public+Sans:wght@300;400;700&display=swap');


body {
  background-color: #f8d6b3;
  font-family: 'Public Sans', sans-serif;
}


.page-enter-active,
.page-leave-active {
  transition: all 0.4s;
}
.page-enter-from,
.page-leave-to {
  opacity: 0;
  filter: blur(1rem);
}



</style>