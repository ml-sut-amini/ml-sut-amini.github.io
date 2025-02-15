<script setup lang="ts">
const sampleTitle = 'Course Description';
const sampleDescription = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas purus viverra accumsan in nisl nisi. Arcu cursus vitae congue mauris rhoncus aenean vel elit scelerisque. In egestas erat imperdiet sed euismod nisi porta lorem mollis. Morbi tristique senectus et netus. Mattis pellentesque id nibh tortor id aliquet lectus proin. Sapien faucibus et molestie ac feugiat sed lectus vestibulum. Ullamcorper velit sed ullamcorper morbi tincidunt ornare massa eget. Dictum varius duis at consectetur lorem. Nisi vitae suscipit tellus mauris a diam maecenas sed enim. Velit ut tortor pretium viverra suspendisse potenti nullam. Et molestie ac feugiat sed lectus. Non nisi est sit amet facilisis magna. Dignissim diam quis enim lobortis scelerisque fermentum. Odio ut enim blandit volutpat maecenas volutpat. Ornare lectus sit amet est placerat in egestas erat. Nisi vitae suscipit tellus mauris a diam maecenas sed. Placerat duis ultricies lacus sed turpis tincidunt id aliquet.';
</script>

<template>
  <div class="section">
    <div class="section-content p-8 sm:p-12 md:p-16 xl:p-20">
      <div class="title font-bold text-3xl sm:text-4xl">{{ sampleTitle }}</div>
      <div class="content text-black-600 text-md md:text-xl lg:text-xl">
        This course provides a comprehensive introduction to Machine Learning, covering foundational concepts and practical applications. Students will explore problem formulation in Machine Learning, working with different types of Supervised/Unsupervised/Reinforcement Learning scenarios, and understanding training and optimization procedures.
      </div>
      <div class="content text-black-600 text-md md:text-xl lg:text-xl">
        The course includes extensive coverage of probability and statistics concepts, with approximately 11 sections dedicated to reviewing these fundamental topics. Through hands-on projects and assignments, students will gain practical experience in implementing various machine learning algorithms and understanding their theoretical foundations.
      </div>
    </div>
  </div>
</template>

<style scoped>
.content {
  font-size: 20px;
  line-height: 1.75rem;
}
</style>