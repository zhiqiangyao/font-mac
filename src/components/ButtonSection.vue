<template>
    <div class="button-section">
      <h2>Button Section</h2>
      <div>
        <button @click="handleButtonClick(1)">Button 1</button>
        <button @click="handleButtonClick(2)">Button 2</button>
        <button @click="handleButtonClick(3)">Button 3</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      handleButtonClick(buttonNumber) {
        // Handle button click logic here
        console.log(`Button ${buttonNumber} clicked.`);
      },
    },
  };
  </script>
  
  <style scoped>
  .button-section {
    flex: 1;
    padding: 20px;
    background-color: #f9f9f9;
  }
  
  .button-section h2 {
    font-size: 24px;
    margin-bottom: 10px;
  }
  
  .button-section button {
    display: block;
    width: 100%;
    padding: 10px;
    font-size: 18px;
    background-color: #333;
    color: #fff;
    border: none;
    margin-bottom: 10px;
    cursor: pointer;
    transition: background-color 0.2s;
  }
  
  .button-section button:hover {
    background-color: #555;
  }
  </style>
  
  