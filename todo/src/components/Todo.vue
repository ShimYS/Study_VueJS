<template>
    <button class="list-group-item text-left"  :key="todo" @click="clickButton">
        {{ label }}
    </button>
</template>
<script>
    export default {
        props: ['label'],
        methods: {
            clickButton() {
                this.$emit('componentClick');
            }
        }
    };
</script>