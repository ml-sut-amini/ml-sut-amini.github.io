<template>
  <footer class="footer-body">
    <div class="copyright">
      <p class="copyright-text" >
        Copyright © 2024 | Department of Electrical Engineering | Sharif University of Technology
      </p>
    </div>
  </footer>
</template>
<script setup lang="ts">
</script>

<style scoped>
.footer-body {
  background-color: transparent;
  padding-top: 20px;
}

.copyright {
  display: flex;
  flex-direction: row-reverse;
  align-items: center;
  justify-content: center;
  border-top: 1px solid rgba(0, 0, 0, 0.2);
  padding-top: 0;
}

.copyright .copyright-text {
  margin: 10px;
  text-align: center;
  color: rgb(94 98 130);
}

@media (min-width: 640px) {
  .footer-body {
    padding: 20px 4rem 1.5rem;
  }
  .copyright-text {
    margin-top: 2rem;
  }
}
</style>