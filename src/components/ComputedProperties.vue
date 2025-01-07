<script setup>
import { computed, ref } from 'vue'
const number = ref(5);

const squareNumber = computed(() => number.value * number.value);

const sq = number.value * number.value;

function increment() {
    number.value++;
}

</script>

<template>
    <h1>Hello</h1>
    <p class="font-bold m-8 p-4">Original number : {{ number }}</p>
    <p class="font-bold m-8 p-4">Squared number : {{ squareNumber }}</p>
    <p class="font-bold m-8 p-4">Squared number : {{ sq }}</p>
    <button @:click="squareNumber" class="bg-cyan-500 hover:bg-cyan-700 text-white font-bold mx-8 py-2 px-4 rounded">Square</button>
    <button v-on:click="increment()" class="bg-blue-500 hover:bg-blue-700 text-white font-bold mx-8 py-2 px-4 rounded">Increment </button>

</template>

<!-- Avec computed, quand on clique sur increment, squareNumber est aussi mis à jour, alors que sq ne l'est pas -->
