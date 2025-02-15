<script setup lang="ts">
const sampleDescription = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas purus viverra accumsan in nisl nisi. Arcu cursus vitae congue mauris rhoncus aenean vel elit scelerisque. In egestas erat imperdiet sed euismod nisi porta lorem mollis. Morbi tristique senectus et netus. Mattis pellentesque id nibh tortor id aliquet lectus proin. Sapien faucibus et molestie ac feugiat sed lectus vestibulum. Ullamcorper velit sed ullamcorper morbi tincidunt ornare massa eget. Dictum varius duis at consectetur lorem. Nisi vitae suscipit tellus mauris a diam maecenas sed enim. Velit ut tortor pretium viverra suspendisse potenti nullam. Et molestie ac feugiat sed lectus. Non nisi est sit amet facilisis magna. Dignissim diam quis enim lobortis scelerisque fermentum. Odio ut enim blandit volutpat maecenas volutpat. Ornare lectus sit amet est placerat in egestas erat. Nisi vitae suscipit tellus mauris a diam maecenas sed. Placerat duis ultricies lacus sed turpis tincidunt id aliquet.';
</script>

<template>
  <div class="sub-section">
    <div class="sub-section-content">
      <div class="title-pack">
<!--        <img src="/icons/warning.png" alt="warning" class="warning-image" />-->
        <div class="title font-bold text-2xl sm:text-2xl md:text-3xl">Course Policy</div>
<!--        <img src="/icons/warning.png" alt="warning" class="warning-image" />-->
      </div>
      <div class="content text-black-600 text-md md:text-xl lg:text-xl">
        {{ sampleDescription }}
      </div>
    </div>
  </div>
</template>

<style scoped>
.sub-section-content .title-pack {
  display: flex;
  flex-direction: row;
  width: 100%;
  margin-bottom: 20px;
  align-items: center;
  justify-content: center;
}

.sub-section-content .title-pack .title {
  color: var(--secondary-color-darker);
  margin: 0 20px;
}

.sub-section-content .content {
  text-align: justify;
  margin-bottom: 10px;
}

.sub-section-content .warning-image {
  height: 35px;
  width: 35px;
}
</style>