<script setup>
import Header from './Header.vue'
import Avatar from './Avatar.vue'
import Title from './Title.vue'
import Tabs from './Tabs.vue'
import PageToolbar from './PageToolbar.vue'
import Button from './Button.vue'
import TaskList from './TaskList.vue'

let tabs = [
  {title: 'List', isActive: true},
  {title: 'Board', isActive: false},
  {title: 'Calendar', isActive: false}
]
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
        <Tabs :tabs="tabs"></Tabs>
      </template>
    </Header>
  </div>
  <PageToolbar>
      <Button></Button>
  </PageToolbar>
  <TaskList/>
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