<template>
  <div class="app">
    <div class="header">
      <img src="path_to_your_image.jpg" alt="Header Image" />
    </div>
    <div class="container">
      <div class="bottom-section">
        <ListSection />
        <ButtonSection />
      </div>
    </div>
  </div>
</template>

<script>
import ListSection from "@/components/ListSection.vue";
import ButtonSection from "@/components/ButtonSection.vue";

export default {
  components: {
    ListSection,
    ButtonSection,
  },
};
</script>

<style>
/* Scoped styles for App.vue */
.app {
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

.header {
  text-align: center;
  padding: 20px;
  background-color: #333;
  color: #fff;
}

.header img {
  max-width: 100%;
  height: auto;
}

.bottom-section {
  display: flex;
}

</style>
