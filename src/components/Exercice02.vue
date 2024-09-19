<template>
    <div id="app">
      <h1 :id="elementId" :class="elementClass">Heading</h1>
    </div>
  </template>
  
  <script setup>
  const elementId = "heading";  
  const elementClass = "heading";  
  </script>
  
  <style scoped>
  .heading {
    color: blue;
    font-size: 24px;
  }
  </style>