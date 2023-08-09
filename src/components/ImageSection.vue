<template>
    <div class="image-section">
      <img :src="imageSrc" alt="Image" />
    </div>
  </template>
  
  <script>
  export default {
    props: {
      imageSrc: {
        type: String,
        required: true,
      },
    },
  };
  </script>
  
  <style scoped>
  .image-section {
    text-align: center;
    margin-top: 20px;
    background-color: #333;
    padding: 20px;
  }

  .image-section img {
    max-width: 100%;
    height: auto;
  }
</style>  