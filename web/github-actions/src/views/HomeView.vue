<script setup>
</script>

<template>
  <div class="calculator">
    <div v-for="n in 9" class="calculator_number"> {{ n }} </div>
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
