<template>
    <div>
      <input type="text" :disabled="true" placeholder="Không cho phép nhập" />
      <p>isDisable=true</p>
  
      <input type="text" :disabled="false" placeholder="Cho phép nhập" />
      <p>isDisable=false</p>
    </div>
  </template>
  
  <script setup>
  </script>
  
  <style scoped>
  input {
    margin-right: 20px;
    margin-bottom: 10px;
  }
  
  p {
    font-weight: bold;
    font-size: 16px;
    margin-top: 0;
  }
  </style>
  