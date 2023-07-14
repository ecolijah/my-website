<script setup>
</script>

<template>
    <ul>
      <li>film 1</li>
      <li>film 2</li>
      <li>film 3</li>
      <li>film 4</li>
    </ul>
</template>
  
<script>
  export default {
    name: 'films'
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
  