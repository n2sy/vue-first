<script setup>
import { ref } from 'vue'
const persons = ref(["Homer", "Lisa", "Bart"]);
const books = ref([
    { id: 1, author: "J.K. Rowling", genre: "Fantasy", year: 1997 },
    { id: 2, author: "J.R.R. Tolkien", genre: "Fantasy", year: 1954 },
    { id: 3, author: "Philip K. Dick", genre: "Science fiction", year: 1968 },
    { id: 4, author: "George Orwell", genre: "Science fiction", year: 1949 },
    { id: 5, author: "Ray Bradbury", genre: "Science fiction", year: 1953 },
]);
const user = ref({
    "id": 1,
    "name": "Leanne Graham",
    "username": "Bret",
    "email": "Sincere@april.biz",
    "address": {
      "street": "Kulas Light",
      "suite": "Apt. 556",
      "city": "Gwenborough",
      "zipcode": "92998-3874",
      "geo": {
        "lat": "-37.3159",
        "lng": "81.1496"
      }
    },
    "phone": "1-770-736-8031 x56442",
    "website": "hildegard.org",
    "company": {
      "name": "Romaguera-Crona",
      "catchPhrase": "Multi-layered client-server neural-net",
      "bs": "harness real-time e-markets"
    }
  })
</script>

<template>
    <!-- <ul class="max-w-md divide-y divide-gray-200 dark:divide-gray-700">
        <li v-for="(person, index) in persons" :key="index" class="pb-3 sm:pb-4 py-3"> {{ index }} -- {{ person }}</li>
        <li v-for="(person, i) in persons" :key="index" class="pb-3 sm:pb-4 py-3"> {{ i }} -- {{ person }}</li>
     
    </ul> -->
    <!-- <ul v-for="({id, author, genre, year}) in books" :key="id"  class="m-8 max-w-md divide-y divide-gray-200 dark:divide-gray-700">
        <li class="pb-3 sm:pb-4 py-3"> {{ author }}</li>
        <li class="pb-3 sm:pb-4 py-3"> {{ genre }}</li>
        <li class="pb-3 sm:pb-4 py-3"> {{ year }}</li>
     
    </ul> -->
    <!-- On peut aussi avoir des v-for imbriqués -->
     
    <!-- Mnt parcourons un objet avec v-for -->
     
    <div v-for="(value, keys, index) in user" :key="idex"  class="m-8 max-w-md divide-y divide-gray-200 dark:divide-gray-700">
        <p> {{ value }}</p>
    </div>
    
    <div v-for="nb in 5">
        <p> {{ nb }}</p>
    </div>
   
</template>
