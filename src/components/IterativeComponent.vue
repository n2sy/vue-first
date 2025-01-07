<script setup>
import { ref } from 'vue'
const persons = ref(["Homer", "Lisa", "Bart"]);
</script>

<template>
    <ul class="max-w-md divide-y divide-gray-200 dark:divide-gray-700">
        <li v-for="(person, index) in persons" :key="index" class="pb-3 sm:pb-4 py-3"> {{ index }} -- {{ person }}</li>
     
    </ul>
    
   
    
</template>
