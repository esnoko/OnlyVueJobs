<script setup>
import { defineProps } from 'vue';

defineProps({
    title: {
        type: String,
        default: 'Become a Vue Dev'
    },

    subtitle: {
        type: String,
        default: 'Find the Vue job that fits your skills and needs'
    }
})
</script>

<template>
    <section class="bg-[#12141c] py-20 border-b border-[#12141c]">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col items-center">
            <div class="text-center">
                <h1 class="text-4xl font-extrabold text-[#e9e3d5] sm:text-5xl md:text-6xl">
                    {{ title }}
                </h1>
                <p class="my-4 text-xl text-[#e9e3d5]">
                    {{ subtitle }}
                </p>
            </div>
        </div>
    </section>
</template>