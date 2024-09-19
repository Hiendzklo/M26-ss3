<template>
    <div>
      <h1>Display Image</h1>
      <img :src="image" alt="Sample Image" />
    </div>
  </template>
  
  <script setup>
  const image = "https://img4.thuthuatphanmem.vn/uploads/2019/12/16/hinh-nen-4k-thien-nhien-dep_024352261.jpg"; 
  </script>
  
  <style scoped>
  img {
    max-width: 100%;
    height: auto;
  }
  </style>
  