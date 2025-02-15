<script setup>
import {ref} from "vue";
import {Dialog, DialogPanel} from "@headlessui/vue";
import {XMarkIcon} from "@heroicons/vue/24/outline";

const mobileMenuOpen = ref(false);

const closeMenu = () => {
  mobileMenuOpen.value = false;
};

const scrollToSection = (sectionId) => {
  const section = document.getElementById(sectionId);

  if (section) {
    const offset = 70;
    const sectionPosition = section.getBoundingClientRect().top + window.scrollY;
    const offsetPosition = sectionPosition - offset;

    window.scrollTo({
      top: offsetPosition,
      behavior: "smooth",
    });
  }
};

</script>


<template>
  <div class="navbar-header header-padding">
    <img src="/sharif-logo-png-transparent.png" alt="logo" style="height: 50px;">
    <div class="inner-navbar">
      <ul class="inner-navbar-list hidden lg-flex">
        <li class="navbar-item" @click="scrollToSection('home')">Home</li>
        <li class="navbar-item" @click="scrollToSection('team')">Team</li>
        <li class="navbar-item" @click="scrollToSection('course')">Course Details</li>
        <li class="navbar-item" @click="scrollToSection('schedule')">Schedule</li>
        <li class="navbar-item" @click="scrollToSection('contact')">Contact</li>
        <!--        <li class="navbar-item"><a href="#" @click.prevent="scrollToSection('home')">Home</a></li>-->
        <!--        <li class="navbar-item"><a href="#" @click.prevent="scrollToSection('team')">Team</a></li>-->
        <!--        <li class="navbar-item"><a href="#" @click.prevent="scrollToSection('course')">Course Details</a></li>-->
        <!--        <li class="navbar-item"><a href="#" @click.prevent="scrollToSection('schedule')">Schedule</a></li>-->
        <!--        <li class="navbar-item"><a href="#" @click.prevent="scrollToSection('contact')">Contact</a></li>-->
      </ul>
    </div>
    <button class="lg-hidden hamburger-button" @click="mobileMenuOpen = true" aria-label="hamburger-button">
      <img src="/menu.png" alt=""/>
    </button>

    <Dialog
        as="div"
        class="lg-hidden"
        @close="mobileMenuOpen = false"
        :open="mobileMenuOpen"
        id="dialog"
    >
      <div class="mini-menu" />
      <DialogPanel
          class="dialog-panel"
      >
        <div class="dialog-panel-inner">
          <a href="#">
            <img src="/sharif-logo-png-transparent.png" alt="logo" style="height: 50px;">
          </a>
          <button
              type="button"
              class="close-button"
              @click="mobileMenuOpen = false"
              aria-label="close"
          >
            <span class="sr-only">Close menu</span>
            <XMarkIcon style="height: 1.5rem; width: 1.5rem;" aria-hidden="true" />
          </button>
        </div>
        <div class="flow-root">
          <div class="flow-root-inner">
            <div class="flow-root-inner-2">
              <div @click.prevent="scrollToSection('home'); closeMenu()" class="flow-item">
                Home
              </div>
              <div @click.prevent="scrollToSection('team'); closeMenu()" class="flow-item">
                Team
              </div>
              <div @click.prevent="scrollToSection('course'); closeMenu()" class="flow-item">
                Course Details
              </div>
              <div @click.prevent="scrollToSection('schedule'); closeMenu()" class="flow-item">
                Schedule
              </div>
              <div @click.prevent="scrollToSection('contact'); closeMenu()" class="flow-item">
                Contact
              </div>
            </div>
          </div>
        </div>
      </DialogPanel>
    </Dialog>
  </div>
</template>

<style scoped>
.navbar-header {
  width: 100%;
  display: flex;
  align-items: center;
  background-color: whitesmoke;
  position: fixed;
  justify-content: space-between;
  z-index: 41;
  padding-top: 0;
  padding-bottom: 0;
  height: 64px;
  box-shadow: rgba(0, 0, 0, 0.24) 0 2px 8px;
}

.inner-navbar {
  display: flex;
  align-items: center;
}

.inner-navbar-list {
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: space-between;
  padding: 15px 0;
}

.navbar-item {
  min-width: fit-content;
  height: 100%;
  font-size: 1.1rem;
  margin-left: 3rem;
  cursor: pointer;
}

.navbar-item::marker {
  content: "";
}

.hidden {
  display: none;
}

.hamburger-button {
  background-color: transparent;
  border: none;
  align-items: center;
  display: flex;
}

.hamburger-button > img {
  width: 40px;
}

.mini-menu {
  position: fixed;
  z-index: 50;
  inset: 0;
}

.header-padding {
  padding-left: 1.25rem;
  padding-right: 1.25rem;
}

.dialog-panel {
  position: fixed;
  z-index: 50;
  width: 100%;
  right: 0;
  top: 0;
  bottom: 0;
  overflow-y: auto;
  --tw-bg-opacity: 1;
  background-color: rgb(255 255 255);
  padding: 1.5rem;
  box-shadow: rgba(0, 0, 0, 0.05) 0 6px 24px 0, rgba(0, 0, 0, 0.08) 0 0 0 1px;
}

.dialog-panel-inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.close-button {
  color: rgb(55 65 81);
  padding: 0.625rem;
  border-radius: 0.375rem;
  cursor: pointer;
  background-color: transparent;
  border: none;
  background-image: none;
}

.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border-width: 0;
}

.flow-root {
  display: flow-root;
}

.flow-root-inner {

}

.flow-root-inner-2 {
  padding-top: 1.2rem;
  padding-bottom: 1.2rem;
}

.flow-root-inner-2 > .flow-item {
  color: rgb(17, 24, 39);
  line-height: 1.6;
  font-weight: 600;
  font-size: 1rem;
  padding: 0.75rem 0;
  border-radius: 0.5rem;
  display: block;
  text-decoration: inherit;
  cursor: pointer;
}

@media (min-width: 900px) {
  .navbar-header {
    justify-content: left;
  }

  .lg-hidden {
    display: none;
  }

  .lg-flex {
    display: flex;
  }
}

@media (min-width: 640px) {
  .header-padding {
    padding-left: 3rem;
    padding-right: 3rem;
  }
  .dialog-panel {
    max-width: 24rem;
  }
}
</style>