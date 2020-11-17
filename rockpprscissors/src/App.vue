<template>
  <div id="app">
   <joke-button></joke-button>
   <div>
     <button @click="selection(1)">Loud</button>
     <button @click="selection(2)">Snake</button>
     <button @click="selection(3)">Normal</button>
   </div>
   <loud-joke v-if="choice ==1"></loud-joke>
   <normal-joke v-if="choice == 3"></normal-joke>
   <snake-joke v-if="choice == 2"></snake-joke>
  </div>
</template>

<script>
import JokeButton from './components/JokeButton.vue';
import LoudJoke from './components/LoudJoke.vue';
import NormalJoke from './components/NormalJoke.vue';
import SnakeJoke from './components/SnakeJoke.vue';

export default {
  name: "App",
  components: {
    JokeButton,
    LoudJoke,
    NormalJoke,
    SnakeJoke
  },
  data: function(){
    return {
      choice: 3
    }
  },
  methods: {
    selection(choice){
      this.choice = choice
    }
  },

};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
