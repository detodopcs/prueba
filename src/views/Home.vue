<template>
  <form>
    <input 
    type="text" class="input"
     placeholder="ingrese nombre"
     v-model="tarea.texto"     
     >

     <div class="form">
       <input type="checkbox" id="check1" v-model="tarea.categorias" value="Javascript"/>
       <label for="check1">Javascript</label>
     </div>
     <div class="form">
       <input type="checkbox" id="check2"  v-model="tarea.categorias" value="Node Js" />
       <label for="check2">Node JS</label>
     </div>
     <div class="form">
       <input type="checkbox" id="check3" v-model="tarea.categorias" value="Vue JS"/>
       <label for="check3">Vue JS</label>
     </div>

     <div class="form-radio"><input type="checkbox" id="radio1" v-model="tarea.estados"
              value="urgente"/>              
              
       <label for="radio1">urgente</label>
     </div>

      <div class="form"><input type="number"  v-model.number="tarea.estados"/> 
       <label for="number"></label>
     </div>

      
  <hr>

  <p>{{tarea}}</p>

    

  </form>
</template>

<script>
export default {

  data() {
    return {
       tarea:{
         nombre:'',
         categorias: [], 
         estados:''
       }

    
    }
  }




}
</script>

<style>

.input{
  width: 100%;
  padding:1 0;
}


</style>