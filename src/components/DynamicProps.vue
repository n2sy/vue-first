<script setup>
const props = defineProps(
    {
        p1 : String,
        p2 : {
            type : String,
            required : true,
            default : "Dupond"
        }   ,
        p3 : {
            type : Number,
            validator : (value) => {
                return value > 20 && value < 50 
            }
        }
    }
);
</script>

<template>
    <div class="text-center text-3xl">Hello {{ p1 }} {{ p2 }} : {{ p3 }} ans</div>
</template>
