<script setup>
defineProps({
  bg: {
    type: String,
    default: "bg-[#eaeaed]" // Ensure this matches Tailwind format
  }
});
</script>

<template>
  <div :class="`${bg} p-6 rounded-lg shadow-md`">
    <slot></slot>
  </div>
</template>
