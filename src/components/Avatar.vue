<script setup>
const props = defineProps({
    avatar: String
})
</script>
<template>
    <div class="avatar">
        {{ avatar }}
    </div>
</template>

<style>
.avatar {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 48px;
    width: 48px;
    border-radius: 50%;
    background-color: #8d84e8;
    color: #fff;
    margin-right: 16px;
}
</style>