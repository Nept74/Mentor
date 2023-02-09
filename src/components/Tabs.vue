<script setup>
const props = defineProps({
    tab1: String,
    tab2: String,
    tab3: String,
    tab4: String
})
</script>
<template>
        <div class="tab selected">
            {{ tab1 }}
        </div>
        <div class="tab">
            {{ tab2 }}
        </div>
        <div class="tab">
            {{ tab3 }}
        </div>
        <div class="tab">
            {{ tab4 }}
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