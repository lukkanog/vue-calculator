<template>
    <button 
        @click="$emit('buttonClick', label)"
        class="button"
        :class="{double, triple, operation}"
    >
        {{label}}
    </button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        label: {},
        operation: {
            type: Boolean,
            default: false
        },
        double: {
            type: Boolean,
            default: false
        },
        triple: {
            type: Boolean,
            default: false
        }
    }
}
</script>

<style>
:root{
    --bg-button: #f0f0f0;
    --border-button: solid 1px #888;
}

.button{
    font-size: 1.4em;
    background-color: var(--bg-button);
    border: none;
    border-right: var(--border-button);
    border-bottom: var(--border-button);
    outline: none;
}

.button:active{
    background-color: #ccc;
}

.double{
    grid-column: span 2;
}

.triple{
    grid-column: span 3;
}

.operation{
    background-color: #fa8320;
    color: #fff;
}

.operation:active{
    background-color: #fa8320cc;
}
</style>