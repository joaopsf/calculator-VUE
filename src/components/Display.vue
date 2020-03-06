<template>
    <div class="display">{{ value }}</div>
</template>

<script>
    export default {
        props: ['value']
    }
</script>

<style lang="scss" scoped>
    .display {
        grid-column: span 4;
        background-color: #0004;
        display: flex;
        justify-content: flex-end;
        align-items: center;
        padding: 20px;
        font-size: 2.1em;
        font-weight: bold;
        overflow: hidden;
    }
</style>