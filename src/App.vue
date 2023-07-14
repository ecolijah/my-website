<script setup>
import shows from "./components/shows.vue"
import music from "./components/music.vue"
import films from "./components/films.vue"
import { ref } from 'vue';

const showShows = ref(false);
const showMusic = ref(false);
const showFilms =  ref(false);

const loadShows = () => {
  showShows.value = true;
  showFilms.value = false;
  showMusic.value = false;
};

const loadFilms = () => {
  showShows.value = false;
  showFilms.value = true;
  showMusic.value = false;
};

const loadMusic = () => {
  showShows.value = false;
  showFilms.value = false;
  showMusic.value = true;
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
            <shows v-if="showShows"></shows>
            <films v-if="showFilms"></films>
            <music v-if="showMusic"></music>
        </div>
    </main>   
</template>

<style scoped>
</style>
