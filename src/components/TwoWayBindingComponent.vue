<script setup>
import { reactive } from 'vue'
const ville = reactive({
    name : "Paris"});
    
    const user = reactive({
        name : "John",
        age : ''   ,
        password : ''
    })
</script>

<template>
    <input type="text" v-model="ville.name">
    {{  ville.name }}
    
    <form @submit.prevent>
        <input type="text" v-model="user.name">
        <input type="number" v-model="user.age">
        <input type="password" v-model="user.password">
        <button>Submit</button>
    </form>
</template>
