<script setup>
import { defineProps } from 'vue';

defineProps({
    bg: {
        type: String,
        default: '#eaeaed'
    }
});
</script>

<template>
    <div div :class="`${bg} p-6 rounded-lg shadow-md`">
        <slot></slot>
    </div>
</template>