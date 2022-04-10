<template>
  <button
      class="btn"
      :class="isActive? 'disabled' : null"
      :disabled="isActive"
  >
    {{ value }}
  </button>
</template>

<script>
export default {
  name: "tButton",
  props: {
    'value': {
      type: String
    },
    'isActive': {
      type: Boolean
    },
  }
}
</script>

<style scoped>
.btn {
  height: 56px;
  width: 100%;
  background-color: #0880AE;
  border-radius: 6px;
  border: none;
  color: #EBF4F8;
  font-size: 16px;
  font-weight: normal;
}

.disabled {
  background-color: #B1B5BF;
  color: #DBE2EA;
}
</style>
