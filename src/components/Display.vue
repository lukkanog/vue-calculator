<template>
    <div class="display">
        {{value}}
    </div>
</template>

<script>
export default {
    name: 'Display',
    props: {
        value: {
            type: String,
            required: true
        }
    },
}
</script>

<style> 
.display{
    grid-column: span 4;
    background-color: #0005;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    padding: 20px;
    font-size: 2.1em;
    overflow: hidden;
    color: #ddd;
}
</style>