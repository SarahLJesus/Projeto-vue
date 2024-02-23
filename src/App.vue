<script setup>
import { ref } from 'vue'

const contador = ref(0)

function decrementar() {
 if (contador.value > 0) {contador.value--}
}

</script>

<template>
<button @click="contador++">+</button>
<button @click="decrementar">-</button>
<p>Valor do contador: {{ contador }}</p>
</template>

<style scoped>
button {
    font-weight: bold;
    background-color: blue;
    color: white;
    border: 0;
}
</style>
