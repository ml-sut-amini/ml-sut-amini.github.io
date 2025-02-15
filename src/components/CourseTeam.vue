<script setup lang="ts">

import PersonCard from "../components/PersonCard.vue";

const sampleTitle = 'Instructor Team';
const courseInstructor = {
  title: 'Course Instructor',
  firstName: 'Sajjad',
  lastName: 'Amini',
  avatar: 'Amini.jpg',
  personalWebsite: 'https://sharif.edu/~s_amini/'
};

const courseHeadAssistants = {
  title: 'Course Head Assistants',
  people: [
    {firstName: 'Borna', lastName: 'Khodabandeh', avatar: 'Khodabandeh.jpg', email: 'borna710kh@gmail.com'},
    {firstName: 'Amir Abbas', lastName: 'Afzali', avatar: 'Afzali.jpg', email: 'amir8afzali@gmail.com'}
  ]
};

const courseAssistants = {
  title: 'Course Assistants',
  people: [
    {firstName: 'Arshak', lastName: 'Rezvani', avatar: 'Rezvani.jpg', personalWebsite: 'https://ir.linkedin.com/in/arshak-rezvani-3b3423218'},
    {firstName: 'Illia', lastName: 'Hashemi Rad', avatar: 'HashemiRad.jpg', personalWebsite: 'https://linkedin.com/in/ilia-hashemi-rad'},
    {firstName: 'Ramtin', lastName: 'Moslemi', avatar: 'Moslemi.jpg', personalWebsite: 'https://ramtinmoslemi.github.io'},
    {firstName: 'Ali', lastName: 'Nikkhah', avatar: 'Nikkhah.jpg', personalWebsite: 'https://ir.linkedin.com/in/alinikkhah2001'},
    {firstName: 'Hesam', lastName: 'Hosseini', avatar: 'Hosseini.jpg', personalWebsite: ''},
    {firstName: 'Homan', lastName: 'Zolfaghari', avatar: 'Zolfaghari.jpg', personalWebsite: 'https://hoomanzolfaghari84.github.io/'},
    {firstName: 'Amir', lastName: 'Mirrashid', avatar: 'Mirrashid.jpg', personalWebsite: ''},
    {firstName: 'Arash', lastName: 'Hajian', avatar: 'Hajian.jpg', personalWebsite: ''},
    {firstName: 'Amir', lastName: 'Afzali', avatar: 'Afzali.jpg', personalWebsite: ''},
    {firstName: 'Ali', lastName: 'Ackbari', avatar: 'Ackbari.jpg', personalWebsite: ''},
    // {firstName: '', lastName: '', avatar: 'profile.jpg', personalWebsite: ''},
    // {firstName: '', lastName: '', avatar: 'profile.jpg', personalWebsite: ''},
    // {firstName: '', lastName: '', avatar: 'profile.jpg', personalWebsite: ''},
  ]
};
</script>

<template>
  <div class="section">
    <div class="section-content">
      <div class="title">{{ sampleTitle }}</div>
      <div class="sub-section">
        <div class="sub-section-content">
          <div class="sub-title">{{ courseInstructor.title }}</div>
          <div class="grid-team">
            <div class="grid-card">
              <PersonCard
                  :firstName="courseInstructor.firstName"
                  :lastName="courseInstructor.lastName"
                  :avatar="courseInstructor.avatar"
                  :personalWebsite="courseInstructor.personalWebsite"
              />
            </div>
          </div>
        </div>
        <div class="sub-section-content">
          <div class="sub-title">{{ courseHeadAssistants.title }}</div>
          <div class="grid-team">
            <div class="grid-card" v-for="(headAssistant, index) in courseHeadAssistants.people" :key="index">
              <PersonCard
                  :firstName="headAssistant.firstName"
                  :lastName="headAssistant.lastName"
                  :avatar="headAssistant.avatar"
                  :personal-website="headAssistant.personalWebsite"
              />
            </div>
          </div>
        </div>
        <div class="sub-section-content">
          <div class="sub-title">{{ courseAssistants.title }}</div>
          <div class="grid-team">
            <div class="grid-card" v-for="(assistant, index) in courseAssistants.people" :key="index">
              <PersonCard
                  :firstName="assistant.firstName"
                  :lastName="assistant.lastName"
                  :avatar="assistant.avatar"
                  :personal-website="assistant.personalWebsite"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.grid-card {
  display: flex;
  flex-direction: column;
}

.grid-team {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1.5rem;
}

@media (min-width: 640px) {
  .grid-team {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }
}

@media (min-width: 768px) {
  .grid-team {
    grid-template-columns: repeat(4, minmax(0, 1fr));
  }
}

@media (min-width: 1024px) {
  .grid-team {
    grid-template-columns: repeat(5, minmax(0, 1fr));
  }
}

@media (min-width: 1280px) {
  .grid-team {
    grid-template-columns: repeat(6, minmax(0, 1fr));
  }
}

</style>