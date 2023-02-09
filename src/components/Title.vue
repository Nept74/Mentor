<script setup>
const props = defineProps({
    title: String
})
</script>
<template>
    <div class="title">
        {{ title }}
    </div>
</template>

<style>

.title {
    min-height: 32px;
    margin-top: 4px;
    align-items: center;
    font-size: 20px;
    line-height: 28px;
    font-weight: 500;
}
</style>