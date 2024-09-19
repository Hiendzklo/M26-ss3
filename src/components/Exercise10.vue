<template>
    <div>
      <h1>Shift + Enter to Submit</h1>
      <!-- Input nhận dữ liệu từ người dùng -->
      <input 
        type="text" 
        placeholder="Nhập văn bản" 
        v-model="inputText" 
        @keydown="handleKeyPress" 
        ref="inputField"
      />
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  // Tạo biến inputText để lưu nội dung nhập
  const inputText = ref('');
  
  // Tạo biến tham chiếu đến input
  const inputField = ref(null);
  
  // Hàm xử lý khi người dùng nhấn Shift + Enter hoặc Enter
  const handleKeyPress = (event) => {
    if (event.key === 'Enter') {
      if (event.shiftKey) {
        // Kiểm tra nếu có nhấn Shift + Enter
        if (inputText.value) {
          alert(inputText.value); // Hiển thị nội dung đã nhập
          inputText.value = ''; // Xóa nội dung trong trường input
          inputField.value.focus(); // Trả con trỏ về trường input
        } else {
          alert('Bạn cần nhập văn bản và nhấn Shift + Enter');
        }
      } else {
        // Nếu chỉ nhấn Enter mà không có Shift
        alert('Bạn cần nhấn Shift + Enter');
      }
    }
  };
  </script>
  
  <style scoped>
  input {
    padding: 10px;
    font-size: 16px;
    width: 300px;
    margin-top: 10px;
  }
  </style>
  