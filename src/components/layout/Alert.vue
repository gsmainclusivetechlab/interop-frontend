<template>
    <div v-if="isVisible" class="sticky-alert">
      {{ message }}
    </div>
  </template>
  
  <script>
  export default {
    name: 'AlertComponent',
    props: {
      message: String,
      isVisible: Boolean
    }
  }
  </script>
  
  <style>
  .sticky-alert {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: #eedca7; /* Yellow background color */
    color: black; /* Text color */
    text-align: center;
    padding: 10px 0;
    z-index: 1000; /* Ensure it sits above other content */
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.3); /* Slight drop shadow */
  }
  </style>
  