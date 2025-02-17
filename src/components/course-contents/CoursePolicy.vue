<script setup lang="ts">
const sectionTitle = 'Course Policies';

const policies = [
  {
    title: 'Attendance',
    content: 'Regular attendance is expected. While attendance is not directly graded, active participation can earn you extra credit.'
  },
  {
    title: 'Late Submissions',
    content: 'Late submissions will be penalized 10% per day up to 3 days. After 3 days, submissions will not be accepted without prior arrangement.'
  },
  {
    title: 'Academic Integrity',
    content: 'All submitted work must be your own. Plagiarism and cheating will result in a failing grade for the assignment and possible disciplinary action.'
  },
  {
    title: 'Communication',
    content: 'Course announcements will be made through the Telegram channel. Important updates will also be posted on the course website.'
  }
];
</script>

<template>
  <div class="section">
    <div class="section-content">
      <div class="title font-bold text-3xl sm:text-4xl">{{ sectionTitle }}</div>
      <div class="sub-section">
        <div class="sub-section-content">
          <div v-for="(policy, index) in policies" :key="index" class="policy-item">
            <h3 class="sub-title font-bold text-2xl sm:text-2xl">{{ policy.title }}</h3>
            <p class="policy-content">{{ policy.content }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.policy-item {
  padding: 1rem 0;
  border-bottom: 1px solid var(--border-color);
}

.policy-item:last-child {
  border-bottom: none;
}

.policy-item h3 {
  color: var(--primary-color);
  margin-bottom: 0.5rem;
}

.policy-content {
  color: var(--text-color);
  line-height: 1.5;
  font-size: 0.95rem;
}
</style>