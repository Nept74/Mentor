<script setup>
const props = defineProps({
    columns: Number
})
</script>

<template>
    <div :class="'table-row grid grid-cols-' + props.columns">
        <slot></slot>
    </div>
</template>

<style>
.table-row{
    border-top: 1px #d4d4d4af solid;
    border-bottom: 1px #d4d4d4af solid;
    min-height: 36px;
}
</style>