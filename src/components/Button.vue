<script setup>
const props = defineProps({
    button: String
})
</script>
<template>
    <div class='my-auto flex flex-row cursor-pointer'>
        <div class="button rounded-l-md bg-blue-600 hover:bg-blue-700">
            {{ button }}
        </div>
        <div class="small-button rounded-r-lg bg-blue-600 hover:bg-blue-700">
            v
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
.button {
    height: 26px;
    width: 80px;
    margin-right: 1px;
    color: white;
}
.small-button {
    height: 26px;
    width: 20px;
    text-align: center;
}
</style>