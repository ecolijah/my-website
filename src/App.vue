<script setup>
import shows from "./components/shows.vue"
import music from "./components/music.vue"
import films from "./components/films.vue"
import { ref } from 'vue';

const showShows = ref(false);
const showMusic = ref(false);
const showFilms =  ref(false);

const loadShows = () => {
  showFilms.value = false;
  showMusic.value = false;
  setTimeout(() => {
    showShows.value = true;
    console.log("here: shows")
  }, 600); // delay in milliseconds, should match the transition duration in your CSS
};

const loadFilms = () => {
  showShows.value = false;
  showMusic.value = false;
  setTimeout(() => {
    showFilms.value = true;
    console.log("here: films")
  }, 600); // delay in milliseconds, should match the transition duration in your CSS
};

const loadMusic = () => {
  showShows.value = false;
  showFilms.value = false;
  setTimeout(() => {
    showMusic.value = true;
    console.log("here: music")
  }, 600); // delay in milliseconds, should match the transition duration in your CSS
};

</script>

<template>
  <h1 class="greeting">Hello.</h1>
    <main class="flex">
        <div class="introduction">
            <div>
                <p>
                    <strong>My name is <span>Elijah Lopez</span></strong>, but you can just call me <strong>Eli</strong>.
                    I'm a Computer Science student who is interested in building technology to promote 
                    sustainability and decentralization. But right now, I just want a job, lol.
                </p>
                <p>
                    I enjoy watching 
                    <a class="animation-link" v-on:click.prevent="loadShows" href="#">tv shows</a> as well as 
                    <a class="animation-link" v-on:click.prevent="loadFilms" href="#">films</a>, 
                    and also listening to 
                    <a class="animation-link" v-on:click.prevent="loadMusic" href="#">music</a>; I believe these to be a great way to express yourself to others. I love sharing my recommendations.
                    Daily physical stimulation is a necessity for me. I enjoy playing competive volleyball and basketball. In addition, becoming more in tune with my body through practicing yoga.
                </p>
                <p>
                    You can find me on 
                    <a href="https://github.com/ecolijah" target="_blank">Github</a>, 
                    <a href="https://www.linkedin.com/in/elijah-lopez-65b809238/" target="_blank">LinkedIn</a>, 
                    and for a more personal platform, 
                    <a href="https://open.spotify.com/user/ecolijah" target="_blank">spotify</a>. 
                    Currently, i dont enjoy social media. Oh and if you need to message me, my 
                    <a href="mailto:elijahlopez@tutanota.com">email</a>.
                </p>
            </div>
        </div>
        <div class = "details">

          <Transition name="slide-fade" mode="out-in">
            <shows v-if="showShows"></shows>
          </Transition>

          <Transition name="slide-fade" mode="out-in">
            <music v-if="showMusic"></music>
          </Transition>

          <Transition name="slide-fade" mode="out-in">
            <films v-if="showFilms"></films>
          </Transition>

        </div>
    </main>   
</template>

<style scoped>
  .slide-fade-enter-active {
    transition: all 0.6s ease-out;
  }

  .slide-fade-leave-active {
    transition: all 0.6s cubic-bezier(1, 0.5, 0.8, 1);
  }

  .slide-fade-enter-from,
  .slide-fade-leave-to {
    transform: translateX(30px);
    opacity: 0;
  }
</style>
