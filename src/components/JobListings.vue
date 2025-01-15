<script setup>
import JobListing from "@/components/JobListing.vue";
import jobData from "@/jobs.json";
import { ref, defineProps } from "vue";

const props = defineProps({
  limit: {
    type: Number,
    default: null,
  },
  showButton: {
    type: Boolean,
    default: false,
  }
});

const jobs = ref(jobData);
</script>

<template>
  <section class="bg-[#e9e3d5] px-4 py-10">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl font-bold text-blue-40 mb-6 text-center">
        Browse Jobs
      </h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <JobListing v-for="job in jobs.slice(0, props.limit || jobs.length)" :key="job.id" :job="job" />
      </div>
    </div>
  </section>
  <section v-if="props.showButton" class="bg-[#e9e3d5] py-10">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8 text-center">
      <a href="/jobs" class="inline-block bg-black text-white text-center py-4 px-6 rounded-xl hover:bg-gray-700">
        View All Jobs
      </a>
    </div>
  </section>
</template>