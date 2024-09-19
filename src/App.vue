<template>
  <div id="app">
    <h1>Bài 1</h1>
    <Exercice01 />
    <h1>Bài 2</h1>
    <Exercice02/>
    <h1>Bài 3</h1>
    <Exercice03/>
    <h1>Bài 4</h1>
    <Exercise04/>
    <h1>Bài 5</h1>
    <Exercise05/>
    <h1>Bài 6</h1>
    <Exercise06/>
    <h1>Bài 7</h1>
    <Exercise07/>
    <h1>Bài 8</h1>
    <Exercise08/>
    <h1>Bài 9</h1>
    <Exercise09/>
    <h1>Bài 10</h1>
    <Exercise10/>
  </div>
</template>

<script setup>
import Exercice01 from './components/Exercice01.vue'; 
import Exercice02 from './components/Exercice02.vue';
import Exercice03 from './components/Exercice03.vue';
import Exercise04 from './components/Exercise04.vue';
import Exercise05 from './components/Exercise05.vue';
import Exercise06 from './components/Exercise06.vue';
import Exercise07 from './components/Exercise07.vue';
import Exercise08 from './components/Exercise08.vue';
import Exercise09 from './components/Exercise09.vue';
import Exercise10 from './components/Exercise10.vue';
</script>

<style scoped>
#app {
  text-align: center;
  margin-top: 50px;
}

h1 {
  font-size: 24px;
  color: #42b983;
}
</style>
