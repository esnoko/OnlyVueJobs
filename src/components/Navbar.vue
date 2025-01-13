<script setup>
import logo from '@/assets/img/logo.png'
</script>

<template>
    <nav class="bg-[#12141c] border-b border-[#12141c]">
        <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
            <div class="flex h-20 items-center justify-between">
                <div class="flex flex-1 items-center justify-center md:items-stretch md:justify-start">
                    <!-- Logo -->
                    <a class="flex flex-shrink-0 items-center mr-4" href="index.html">
                        <img class="h-10 w-auto" :src="logo" alt="Vue Jobs" />
                        <span class="hidden md:block text-[#e9e3d5] text-2xl font-bold ml-2">OnlyVueJobs</span>
                    </a>
                    <div class="md:ml-auto">
                        <div class="flex space-x-2">
                            <a href="index.html"
                                class="text-[#033043] bg-[#e9e3d5] hover:bg-[#eb4a4a] hover:text-white rounded-md px-3 py-2">Home</a>
                            <a href="jobs.html"
                                class="text-[#e9e3d5] hover:bg-[#eb4a4a] hover:text-white rounded-md px-3 py-2">Jobs</a>
                            <a href="add-job.html"
                                class="text-[#e9e3d5] hover:bg-[#eb4a4a] hover:text-white rounded-md px-3 py-2">Add Job</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>