<template>
    <button class="button"
        @click="$emit('onClick', label)"
        :class="{ operation, double, triple }">
        {{ label }}
    </button>
</template>

<script>
    export default {
        props: {
            label: {},
            operation: { type: Boolean },
            double: { type: Boolean },
            triple: { type: Boolean }
        }
    }
</script>

<style lang="scss" scoped>
    @import '../assets/scss/variables.scss';
    .button {
        font-size: 1.4em;
        font-weight: bold;
        background-color: $bg-button;
        border: none;
        border-right: $border-button;
        border-bottom: $border-button;
        outline: none;
        &:active {
            background-color: $bg-active;
        }
        &.double {
            grid-column: span 2;
        }
        &.triple {
            grid-column: span 3;
        }
        &.operation {
            background-color: $bg-operation;
            color: $white;
            &:active {
                background-color: $bg-operation-click;
            }
        }
    }
</style>