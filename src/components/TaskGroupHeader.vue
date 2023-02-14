<template>
    <TableCell>
        <div class="image-container">
            <img src="../assets/arrow_drop_down.svg"/>
        </div>
        <slot></slot>
    </TableCell>
</template>

<script setup>
import TableCell from './TableCell.vue';
</script>


<style scoped child-component="TableCell">
.element:last-child {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    padding-left: 5px;
    font-size: 16px;
    color: black;
    font-weight: 500;
    height: 50px;
}
.image-container{
    margin-right: 4px;
}
.image-container:hover{
    background-color: rgb(218, 218, 218);
}
img{
    width: 30px;
    height: 30px;
}
</style>