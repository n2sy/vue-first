<script setup>
const pseudo = defineProps(["name", "age"])
console.log(pseudo);
pseudo.name = "Mary"; // Impossible de modifier un props. Il est immutable

</script>

<template>

<h1> {{  pseudo.name }} et j'ai {{ pseudo.age }} ans</h1>
</template>
