<script setup>
</script>

<template>
  <div>
    <h2 class="heading">Recent Show Picks:</h2>
    <ul>
      <li>
        <div class="image-container">
          <a href ="https://www.imdb.com/title/tt4288182/" target="_blank">
            <img alt="atlanta" src="../assets/images/paperboy.jpg">
            <div class="overlay">
              <h2>Atlanta</h2>
            </div>
          </a>
        </div>
        <div class = "description">
          <div>
            <p>One of my favorite shows of all time.</p>
          </div>
        </div>
      </li>
      <li>
        <div class="image-container">
          <a href ="https://www.imdb.com/title/tt8531222/?ref_=ttmi_tt" target="_blank">
            <img alt="dave" src="../assets/images/dave.jpg">
            <div class="overlay">
              <h2>Dave</h2>
            </div>
          </a>
        </div>
        <div class = "description">
          <div>
            <p>Absolutely hilarious, with a bunch of wildly-creative cameos.</p>
          </div>
        </div>
      </li>
      <li>
        <div class="image-container">
          <a href ="https://www.imdb.com/title/tt5348176/?ref_=fn_al_tt_1" target="_blank">
            <img alt="barry" src="../assets/images/barry.jpg">
            <div class="overlay">
              <h2>Barry</h2>
            </div>
          </a>
        </div>
        <div class = "description">
          <div>
            <p>A <strong>very</strong> dark comedy.</p>
          </div>
        </div>
      </li>
        <li>
        <div class="image-container">
          <a href ="https://www.imdb.com/title/tt14452776/" target="_blank">
            <img alt="the-bear" src="../assets/images/the-bear.jpg">
            <div class="overlay">
              <h2>The Bear</h2>
            </div>
          </a>
        </div>
        <div class = "description">
          <div>
            <p>I aspire to love what i do as much as chefs.</p>
          </div>
        </div>
      </li>
    </ul>
  </div>
    
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
    padding: 2px 0px;

    font-size: 1.2em;
    color: rgb(255, 255, 255);
  }
  img {
    height: 128px;
    width: auto;
    border-radius: 1%;
    /* border: 1px solid #222222;  */
    /* box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);  */
    
  }

  .heading {
    font-size: var(--normal-font);
    color: var(--text-color);
    margin-top: 0;
  }
  .image-container {
    position: relative;
    display: inline-block;
    left: 0;
    -webkit-transition: left .2s ease-out;
    transition: left .2s ease;
    
  }

  .overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgba(10, 6, 12, 0.621);
  opacity: 0;
  transition: opacity 0.4s ease;
  max-height: 130px;

  }

  .image-container:hover {
    left: -10px;
  }

  .overlay h2 {
  color: var(--link-color);
  font-size: var(--large-font);
  text-align: center;
  text-shadow: 0 0 5px var(--link-color), 
               0 0 10px var(--link-color), 
               0 0 15px var(--link-color)
}

.image-container:hover .overlay {
  opacity: 1;
}

.image-container:hover .overlay p {
  display: block;
}

p {
  color: var(--text-color);
  font-size: var(--small-font);
}

a {
  color: var(--text-color);

}

.description {
  margin-left: 20px;
}


</style>
  