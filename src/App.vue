<template>  
  <Navbar/>

<router-link to="/">
  formularios

</router-link>

<div class="flex">
  <router-link to="/">
    tareas nueva
  </router-link>

</div>

<router-view/>




</template>

<script>
import Navbar from './components/Navbar'


export default { 

components: {
  Navbar
}


}
</script>

<style>

</style>