<script setup>
import Header from './Header.vue'
import Avatar from './Avatar.vue'
import Title from './Title.vue'
import Tabs from './Tabs.vue';
</script>
<template>
  <div class="topbar">
    <Header class="header flex-container">
      <template #avatar>
        <Avatar avatar="MA"></Avatar>
      </template>
      <template #title>
        <Title title="My Tasks"></Title>
      </template>
      <template #tabs>
        <Tabs tab1="List" tab2="Board" tab3="Calendar" tab4="Files"></Tabs>
      </template>
    </Header>
  </div>
</template>

<style scoped>
.topbar {
  border-bottom: 1px #edeae9af solid;
  width: 100%;
  height: 72px;
}

.header {
  padding: 0 24px;
}
.title {
    display: flex;
    flex-direction: row;
}
</style>