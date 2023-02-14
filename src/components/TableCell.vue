<template>
    <div class="element">
        <slot></slot>
    </div>
</template>

<script setup>
const props = defineProps({
    headings: Array
})
</script>

<style scoped>
.element {
    display: flex;
    border-left: 1px #edeae9af solid;
    border-right: 1px #edeae9af solid;
    padding-left: 5px;
    font-size: 14px;
    color: black;
    overflow: hidden;
    white-space: nowrap;
    align-items: center;
}
.element:first-child{
    border-left: 0px white solid;
}
.element:last-child{
    border-right: 0px white solid;
    justify-content: center;
}
</style>