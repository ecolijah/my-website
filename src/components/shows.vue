<script setup>
</script>

<template>
    <ul>
      <li>
        <div>
          <a class="show-image" href = "show1" >
            <img alt="atlanta" src="../assets/images/atlanta.svg">
          </a>
        </div>
        <div class = "description">
          <a href="show1">Atlanta - Donald Glover
          </a>
          <div>
            <p>One of my favorite shows of all time, currently re-watching it and loving it even more</p>
          </div>
        </div>
      </li>
      <li>
        <div>
          <a class="show-image" href = "show1" >
            <img alt="atlanta" src="../assets/images/atlanta.svg">
          </a>
        </div>
        <div class = "description">
          <a href="show1">Atlanta - Donald Glover
          </a>
          <div>
            <p>One of my favorite shows of all time, currently re-watching it and loving it even more</p>
          </div>
        </div>
      </li>
      <li>
        <div>
          <a class="show-image" href = "show1" >
            <img alt="atlanta" src="../assets/images/atlanta.svg">
          </a>
        </div>
        <div class = "description">
          <a href="show1">Atlanta - Donald Glover
          </a>
          <div>
            <p>One of my favorite shows of all time, currently re-watching it and loving it even more</p>
          </div>
        </div>
      </li>
      <li>
        <div>
          <a class="show-image" href = "show1" >
            <img alt="atlanta" src="../assets/images/atlanta.svg">
          </a>
        </div>
        <div class = "description">
          <a href="show1">Atlanta - Donald Glover
          </a>
          <div>
            <p>One of my favorite shows of all time, currently re-watching it and loving it even more</p>
          </div>
        </div>
      </li>
    </ul>
</template>
  
<script>
  export default {
    name: 'shows'
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
  ul {
    list-style-type: none;
    padding: 0 0;
    margin: 0;
  }
  
  li {
    display: flex;
    padding: 10px 10px;
    font-size: 1.2em;
    color: rgb(255, 255, 255);
  }
  img {
    height: auto;
    width: 64px;
    border-radius: 10%;
    border: 1px solid #e64444; 
    box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2); /* Adds a shadow */
    
  }
  .show-image {
    position: relative;
    -webkit-transition:.2s ease-in-out;
    transition:.2s ease-in-out
    
  }

  .show-image:hover {
    top: -10px;
  }

  p {
    color: var(--text-color);
    font-size: var(--small-font);
  }
  
  a {
    color: var(--text-color)
  }

  .description {
    margin-left: 20px;
  }


</style>
  