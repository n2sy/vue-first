<template>
    <!-- <h4 :class="$style['c-1']">Another Module Style</h4>
    <h4 v-bind:class="$style.c2">Another Another Module Style</h4> -->
    <h4 :class="myModule['c-1']">Another Module Style</h4>
    <h4 v-bind:class="myModule.c2">Another Another Module Style</h4>
</template>

<style module="myModule">
    .c-1 {
        background : pink;
        color : grey;
    }
    .c2 {
        background : fuchsia;
        color : yellowgreen;
    }

</style>
