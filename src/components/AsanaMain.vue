<script setup>

import MyTasks from './MyTasks.vue';
import PageToolbar from './PageToolbar.vue';

</script>

<template>
    <div class="mainMenu">
      <MyTasks></MyTasks>
      <PageToolbar></PageToolbar>
    </div>
  </template>
  
  <style scoped>
  .mainMenu {
    float: right;
    background-color:white;
    width: calc(100% - 240px);
    height: calc(100% - 48px);
  }

  </style>
  