<script setup>
// Fetch data from the dogs API endpoint
const { data } = await useFetch("/api/dogs");
// clean up the data
const breeds = data;
//console.log(breeds)
</script>
<template>
  <main>
    <header>
      <h1>Dog Breeds</h1>
    </header>
    <div>
      <ul>
        <!-- Loop through the data to show all dog breeds -->
        <li v-for="breed in breeds" :key="breed.id">
          <!-- TODO: Extract breed name from key in k/v pairs -->
         <h1> {{ breed }}</h1>
         <pre></pre>
        </li>
      </ul>
    </div>
  </main>
</template>
