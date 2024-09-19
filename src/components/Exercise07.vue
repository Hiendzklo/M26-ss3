<template>
    <div>
      <h1>Form</h1>
      <form @submit.prevent="handleSubmit">
        <input type="text" placeholder="Enter something" />
        <button type="submit">Submit</button>
      </form>
    </div>
  </template>
  
  <script setup>
  const handleSubmit = (event) => {
    console.log("Form submission prevented!");
  };
  </script>
  
  <style scoped>
  form {
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  input {
    padding: 5px;
    margin-right: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  
  button {
    padding: 5px 10px;
    font-size: 14px;
    cursor: pointer;
  }
  </style>
  