<template>
    <TableCell>
        <slot></slot>
    </TableCell>
</template>

<script setup>
import TableCell from './TableCell.vue';
</script>


<style scoped child-component="TableCell">
.element {
    display: flex;
    align-items: center;
    padding-left: 5px;
    font-size: 12px;
    color: #7a7a7af5;
}
</style>

