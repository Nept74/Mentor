<template>
    <header>
        <div class="avatarbox">
            <slot name="avatar"></slot>
        </div>
        <div class="column">
            <div class="title">
                <slot name="title"></slot>
            </div>
            <div class="flex flex-row">
                <slot name="tabs"></slot>
            </div>
        </div>
    </header>
</template>

<style scoped>
.avatarbox {
    margin: auto 0;
}
.column {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    box-sizing: border-box;
    flex: 1;
}

</style>