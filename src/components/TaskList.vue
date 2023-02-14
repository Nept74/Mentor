<script setup>
import TableRowVue from "./TableRow.vue"
import TableCell from './TableCell.vue'
import TableHeaderCell from "./TableHeaderCell.vue";
import TaskGroupHeader from "./TaskGroupHeader.vue";

let headings = [
    'Task name', 'Due date', 'Project', 'Executor', '+'
]
let task1 = [
    'Написать список задач', "11.02.2023", "Асана", "Михаил Апанасов", " "
]
let task2 = [
    'Запланировать организационное совещание', '15.02.2023', 'project', 'asdf', ' '
]
let line = ['Recently added']
let line1 = ['Do today']
let line2 = ['Do later']
</script>
<template>
    <TableRowVue :columns="task1.length">
        <TableHeaderCell v-for="prop in headings">
            {{ prop }}
        </TableHeaderCell>
    </TableRowVue>
    <TableRowVue :columns="line.length">
        <TaskGroupHeader v-for="prop in line">
            {{ prop }}
        </TaskGroupHeader>
    </TableRowVue>
    <TableRowVue :columns="task1.length">
        <TableCell v-for="prop in task1">
            {{ prop }}
        </TableCell>
    </TableRowVue>
    <TableRowVue :columns="task1.length">
        <TableCell v-for="prop in task2">
            {{ prop }}
        </TableCell>
    </TableRowVue>
    <TableRowVue :columns="line1.length">
        <TaskGroupHeader v-for="prop in line1">
            {{ prop }}
        </TaskGroupHeader>
    </TableRowVue>
    <TableRowVue :columns="line2.length">
        <TaskGroupHeader v-for="prop in line2">
            {{ prop }}
        </TaskGroupHeader>
    </TableRowVue>
</template>


<style scoped>

</style>