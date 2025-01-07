

<!-- <script setup>
import { reactive } from 'vue'
let initialState = reactive({count : 10})

function affectation() {
    // Reactive cannot be reassigned
    initialState = {count : 20}
}
</script>

<template>
    <h1>Count : {{  initialState.count }}</h1>
    <button @click="initialState.count++" class="bg-cyan-500 hover:bg-cyan-700 text-white font-bold mx-8 py-2 px-4 rounded">Add 1</button>
    <button @click="affectation()" class="bg-cyan-500 hover:bg-cyan-700 text-white font-bold mx-8 py-2 px-4 rounded">Affectation</button>
</template> -->
<script setup>
import { reactive, ref } from 'vue'
let friends = reactive([ref("Nidhal"), ref("Alex"), ref("Mary")])


</script>

<template>
    <h1>{{  friends }}</h1>
    <button @click="friends[0].value = 'John'" class="bg-cyan-500 hover:bg-cyan-700 text-white font-bold mx-8 py-2 px-4 rounded">Change friend</button>
</template>
