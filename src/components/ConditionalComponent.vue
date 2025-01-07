<script setup>
import { ref } from 'vue'
const isTrue = true;
const isFalse = true;
const n = 4;

const isVisible = ref(false)

function toggleIsVisible() {
    isVisible.value = !isVisible.value
}
</script>

<template>
    <div class="bg-green-200 font-bold m-8 p-4 text-center text-3xl">
        <!-- <p v-if="isTrue">This will show if isTrue is true</p>
        <p v-else-if="isFalse">This will show if isTrue is false</p> -->
        
        <!-- <p v-if="n == 1">This n is equal to 1</p>
        <p v-else-if="n == 2">This n is equal to 2</p>
        <p v-else-if="n == 3">This n is equal to 3</p>
        <p v-else>This n is equal to nothing</p> -->
        <p v-show="isVisible">v-show Test</p>
        <button @:click="isVisible = !isVisible" class="bg-cyan-500 hover:bg-cyan-700 text-white font-bold mx-8 py-2 px-4 rounded">Toggle</button>
        <button @:click="toggleIsVisible" class="bg-cyan-500 hover:bg-cyan-700 text-white font-bold mx-8 py-2 px-4 rounded">Toggle</button>
    </div>
</template>
