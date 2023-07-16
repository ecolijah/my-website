<script setup>
</script>

<template>

    <div>
        <h2>Some of my current favorites:</h2>
        <iframe style="border-radius:12px" 
        src="https://open.spotify.com/embed/playlist/192dawcEbGBMDwhERl3gAE?utm_source=generator&theme=0" 
        width="70%" height="570" frameBorder="0" 
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
    </div>

</template>
  
<script>
  export default {
    name: 'music'
  }
</script>
  
<style scoped>
  :root {
    --bg-color: #202124;
    --text-color: #b1bbb3;
    --text-color-light: #9aa0a6;
    --link-color: #7ef062;
    --link-color-hover: #fff;
    --name-color: #d29fec;

    --small-font: 12px;
    --normal-font: 20px;
    --large-font: 64px;  
    
    --gradient-1: #231523;
    --gradient-2: #000000;
  }

  h2 {
    margin-top: 0;
    color: var(--text-color);
    font-size: var(--normal-font);
  }
  
</style>
  