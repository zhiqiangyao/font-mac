<template>
    <div class="list-section">
      <h2>List Section</h2>
      <ul>
        <li v-for="item in items" :key="item.id">{{ item.name }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        items: [
          { id: 1, name: "Item 1" },
          { id: 2, name: "Item 2" },
          { id: 3, name: "Item 3" },
          // Add more items as needed
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .list-section {
    flex: 2;
    padding: 20px;
    background-color: #fff;
    border-right: 1px solid #ccc;
  }
  
  .list-section h2 {
    font-size: 24px;
    margin-bottom: 10px;
  }
  
  .list-section ul {
    list-style: none;
    padding: 0;
  }
  
  .list-section li {
    font-size: 18px;
    margin-bottom: 8px;
  }
  </style>
  
  