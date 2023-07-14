<script setup>
</script>

<template>
    <ul>
      <li>The Mandalorian</li>
      <li>Stranger Things</li>
      <li>The Witcher</li>
      <li>Breaking Bad</li>
    </ul>
</template>
  
<script>
  export default {
    name: 'shows'
  }
</script>
  
<style scoped>
  ul {
    list-style-type: none;
    padding: 0;
  }
  
  li {
    padding: 10px 0;
    font-size: 1.2em;
    color: rgb(255, 255, 255);
  }
</style>
  