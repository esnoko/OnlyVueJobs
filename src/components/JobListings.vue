<script setup>
import JobListing from "@/components/JobListing.vue";
import jobData from "@/jobs.json";
import { ref } from "vue";

const jobs = ref(jobData);
</script>

<template>
  <section class="bg-[#e9e3d5] px-4 py-10">
    <div class="container-xl lg:container m-auto">
      <h2 class="text-3xl font-bold text-blue-40 mb-6 text-center">
        Browse Jobs
      </h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <JobListing v-for="job in jobs" :key="job.id" :job="job" />
      </div>
    </div>
  </section>
</template>
