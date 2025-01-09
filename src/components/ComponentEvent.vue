<script setup></script>

<template>
    <div>
    <button @click="$emit('mary')" class="bg-cyan-500 hover:bg-cyan-700 text-white font-bold mx-8 py-2 px-4 rounded">Change Prenom</button>
    <button @click="$emit('maryevent', 'maaaaaary', 30)" class="bg-cyan-500 hover:bg-cyan-700 text-white font-bold mx-8 py-2 px-4 rounded">Change Prenom II</button>
</div>
</template>
