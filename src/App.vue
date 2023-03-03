<script >
   export default {
  data() {
    return {
      contador: 10
    }
  },
  methods: {
    incrementarContador() {
      this.contador++
    },
    decrementarContador() {
      if(this.contador > 0)
      this.contador--
    }
  },
  resetar(){
    this.contador = 0
  }
  mounted() {
    console.log(`O valor inicial do contador é ${this.contador}.`)
  }
}

</script>

<template>
  <button @click="resetar">C</button>
  <button @click="incrementarContador">Incrementar</button>
  <button @click="decrementarContador">Decrementar</button>
  <p>Valor do contador é: {{ contador }}</p>
</template>

<style scoped>
button {
  font-weight: bold;
}
</style>

