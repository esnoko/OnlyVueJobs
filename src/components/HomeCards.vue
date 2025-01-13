<script setup>
import Card from "./Card.vue";
</script>

<template>
  <section class="bg-[#e9e3d5] py-4">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-4 p-4 rounded-lg">
        <Card>
          <h2 class="text-2xl font-bold text-[#0e0f16]">For Developers</h2>
          <p class="mt-2 mb-4 text-[#0e0f16]">
            Browse our Vue jobs and start your career today
          </p>
          <a
            href="jobs.html"
            class="inline-block bg-[#0e0f16] text-white rounded-lg px-4 py-2 hover:bg-opacity-90"
          >
            Browse Jobs
          </a>
        </Card>
        <Card bg="bg-[#979aa5]">
          <h2 class="text-2xl font-bold text-[#0e0f16]">For Employers</h2>
          <p class="mt-2 mb-4 text-[#0e0f16]">
            List your job to find the perfect developer for the role
          </p>
          <a
            href="add-job.html"
            class="inline-block bg-[#0e0f16] text-white rounded-lg px-4 py-2 hover:bg-opacity-90"
          >
            Add Job
          </a>
        </Card>
      </div>
    </div>
  </section>
</template>
