<script setup>
</script>

<template>
    <div>
      <h2 class="heading">Recent Film Picks:</h2>
      <ul>
        <li>
          <div class="image-container">
            <a href ="https://www.imdb.com/title/tt0317248/" target="_blank">
              <img alt="city-of-god" src="../assets/images/city-of-god.jpg">
              <div class="overlay">
                <h2>City of God</h2>
              </div>
            </a>
          </div>
          <div class = "description">
            <div>
              <p>One of my favorite films of all time.</p>
            </div>
          </div>
        </li>
        <li>
          <div class="image-container">
            <a href ="https://www.imdb.com/title/tt0362270/?ref_=nv_sr_srsg_0_tt_5_nm_0_q_the%2520life%2520aquatic" target="_blank">
              <img alt="the-life-aquatic" src="../assets/images/the-life-aquatic.jpg">
              <div class="overlay">
                <h2>The Life Aquatic</h2>
              </div>
            </a>
          </div>
          <div class = "description">
            <div>
              <p>The most amazing soundtrack.</p>
            </div>
          </div>
        </li>
        <li>
          <div class="image-container">
            <a href ="https://m.imdb.com/title/tt0364569/?ref_=fn_al_tt_1" target="_blank">
              <img alt="oldboy" src="../assets/images/oldboy.jpg">
              <div class="overlay">
                <h2>Oldboy</h2>
              </div>
            </a>
          </div>
          <div class = "description">
            <div>
              <p>Not soemthing you see everyday.</p>
            </div>
          </div>
        </li>
          <li>
          <div class="image-container">
            <a href ="https://m.imdb.com/title/tt2543164/?ref_=fn_al_tt_1" target="_blank">
              <img alt="arrival" src="../assets/images/arrival.jpg">
              <div class="overlay">
                <h2>Arrival</h2>
              </div>
            </a>
          </div>
          <div class = "description">
            <div>
              <p>An extremely immersive experience.</p>
            </div>
          </div>
        </li>
      </ul>
    </div>
      
  </template>
  
<script>
  export default {
    name: 'films'
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
  flex-direction: column;
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