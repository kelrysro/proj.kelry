<script >
export default {
  data(){
    return{
      contador:0
    }
  },
  methods: {
    encrementadorContador(){
      this.contador++
    },
    decrementarContador() {
      this.contador--
    },
    
  }
}

</script>

<template>
    <button @click="incrementarContador">Incrementar</button>
    <button @click="decrementarContador">Decrementar</button>
    <p>Valor do contador é: {{ contador }}</p>
</template>

<style scoped >
  button {
    font-weight: bold;
  }
</style>
