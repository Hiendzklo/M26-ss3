<template>
    <div>
      <h1>Link Checker</h1>
      <a href="http://www.google.com" @click.prevent="checkLink">Visit Google (Invalid URL)</a>
    </div>
  </template>
  
  <script setup>
  const checkLink = (event) => {
    const url = event.target.href;
    
    if (!url.startsWith("https://")) {
      alert("Đường dẫn không hợp lệ"); // Hiển thị thông báo nếu đường dẫn không hợp lệ
      event.preventDefault(); // Ngăn chặn hành vi chuyển hướng nếu đường dẫn không hợp lệ
    } else {
      console.log("Đường dẫn hợp lệ, chuyển hướng đến:", url);
    }
  };
  </script>
  
  <style scoped>
  a {
    font-size: 16px;
    color: blue;
    text-decoration: none;
    border: 1px solid #ccc;
    padding: 5px 10px;
    border-radius: 4px;
  }
  
  a:hover {
    background-color: #f0f0f0;
  }
  </style>
  