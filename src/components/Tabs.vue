<script setup>
const props = defineProps({
    tabs: Array
})
</script>
<template>
    <div class="tab" 
    :class="{ selected: tab.isActive }" 
    v-for="tab in tabs"> 
        
        {{ tab.title }}
    </div>
</template>

<style scoped>
.tab {
    margin: 5px 24px 10px 0;
    padding-bottom: 7px;
    font-size: 14px;
    font-weight: 500;
    color: rgb(114, 114, 114);
}

.selected {
    color: black;
    border-bottom: 2px black solid;
}

</style>