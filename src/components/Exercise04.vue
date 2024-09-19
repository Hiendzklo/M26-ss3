<template>
    <div>
      <div :class="{ active: isActive }" :style="{ backgroundColor: backgroundColor }" class="block">
        Block
      </div>
      <p>isActive=true</p>
      <div :class="{ active: false }" :style="{ backgroundColor: backgroundColor }" class="block">
        Block
      </div>
      <p>isActive=false</p>
    </div>
  </template>
  
  <script setup>
  const isActive = true; 
  const backgroundColor = 'blue'; 
  </script>
  
  <style scoped>
  .block {
    width: 150px;
    height: 50px;
    margin-right: 20px;
    text-align: center;
    line-height: 50px;
  }
  
  .active {
    color: #fff; 
  }
  
  div {
    display: inline-block;
  }
  p {
    font-weight: bold;
    font-size: 16px;
    margin-top: 0;
  }
  </style>
  