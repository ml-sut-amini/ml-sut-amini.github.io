<script setup lang="ts">
import CourseDetails from "../course-contents/CourseDetails.vue";
import ClassDetails from "../course-contents/ClassDetails.vue";
</script>

<template>
  <div class="section">
    <div class="section-content p-8 sm:p-12 md:p-16 xl:p-20">
      <div class="title font-bold text-3xl sm:text-4xl">Course Details</div>
      <CourseDetails />
      <ClassDetails />
    </div>
  </div>
</template>

<style scoped>
</style>