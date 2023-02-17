<script>
  export default  {
    data: () => ({
      contador: 10
    }),

    methods: {
      saludar(){
        console.log('Hello')
      },

      increment() {
        this.contador++;
      },

      decrement() {
        this.contador--;
      },

      reset() {
        this.contador = 0;
      }
    }
  }
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo vue" width="125">
    <h1>Hello world from vue</h1>
    <hr />
    <h2>Counter: {{ contador }}</h2>
    <button @click="increment()">+1</button>
    <button @click="decrement()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
</template>

<style scoped>
  h1 {
    font-weight: bolder;
  }
  .container {
    margin: 20px;
    text-align: center;
  }
</style>



