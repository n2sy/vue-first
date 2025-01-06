
<script setup>
const myMessage = "I am nidhal ";
const add = (x, y) => x + y;
const image = "https://files.softicons.com/download/tv-movie-icons/the-simpsons-icon-pack-1-by-jonathan-rey/png/256x256/Homer%20Simpson%2004%20-%20Happy.png";
const cl = { backgroundColor : "red" };

const imageInfos = {
    src : "https://files.softicons.com/download/tv-movie-icons/the-simpsons-icon-pack-1-by-jonathan-rey/png/256x256/Homer%20Simpson%2004%20-%20Happy.png",
    alt : "Alternative text",
    width : "100px",
    height : "100px"
}

</script>

<template>
    <h1>Nested component</h1>
    <h2>{{myMessage}}</h2>
    <h3> 4 + 2 = {{ add(4,2) }}</h3>
    <!-- <img v-bind:src="image"> -->
    <img :src="image">
    <div :style="cl">aaaaa</div>
    
    <img :="imageInfos">

</template>


