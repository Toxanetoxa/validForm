<template>
  <div class="select">
    <div class="select-controls"></div>
  </div>
</template>

<script>
export default {
  name: "tSelect"
}
</script>

<style scoped>
.select {
  width: 100%;
}

.select-controls {
  min-height: 21px;
  padding: 16px 0 15px 16px;
  border: 1px solid #DBE2EA;
  border-radius: 6px;
}

.select-controls:hover {
  border: 1px solid #0880AE;
}
</style>
