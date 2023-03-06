<script setup >
   import { ref } from 'vue' 
   const contador = ref(10)

   function incrementar(){
    contador.value++
   }

   function decrementar(){
    if(contador.value > 0 ){
      contador.value--
    }
   }

   function resetar(){
    contador.value = 0
   }

</script>

<template>
  
  <button @click="incrementarContador">Incrementar</button>
  <button @click="decrementarContador">Decrementar</button>
  <button @click="resetar">C</button>
  <p>Valor do contador é: {{ contador }}</p>
</template>

<style scoped>
button {
  font-weight: bold;
}
</style>

