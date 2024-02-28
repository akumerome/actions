<script>
export default {
  data() {
    return {
      message: '',
    };
  },
  methods: {
    changeNumber(n) {
      console.log(n);
      this.message = n;
    },
  },
};
</script>


<template>
  <p>El número seleccionat és {{ message }}</p>
  <div class="calculator">
    <button v-for="n in 9" :key="n" class="calculator_number" v-on:click="changeNumber(n)">
      {{ n }}
    </button>
  </div>
</template>


<style>
.calculator {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}


.calculator_number {
  border: 1px solid black;
  width: 75px;
  height: 75px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
