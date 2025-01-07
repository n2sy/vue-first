

<script setup>
import { ref } from 'vue';
let count = ref(0);

function increment() {
    console.log(count);
    
    count.value++;
}

function sayHello() {
    console.log("Hello");
    
}
</script>

<template>
    <h1 class="font-bold text-2xl m-8 p-4">Count : {{ count }}</h1>
    
    <!-- Ca marche pas car Vue exige la réactivité pour mettre à jour l'UI -->
    <button v-on:click="increment()" class="bg-blue-500 hover:bg-blue-700 text-white font-bold mx-8 py-2 px-4 rounded">Increment I</button>
    <button v-on:click="count++" class="bg-green-500 hover:bg-green-700 text-white font-bold mx-8 py-2 px-4 rounded">Increment II</button>
    <button @:click="count++" class="bg-pink-500 hover:bg-red-700 text-white font-bold mx-8 py-2 px-4 rounded">Increment III</button>
    <button @:click="sayHello" class="bg-yellow-500 hover:bg-yellow-700 text-white font-bold mx-8 py-2 px-4 rounded">Hello</button>
    
</template>
