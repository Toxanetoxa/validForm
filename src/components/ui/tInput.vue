<template>
  <input class="input" :placeholder="placeholder"/>
</template>

<script>
export default {
  name: "tInput",
  props: ['placeholder']
}
</script>

<style scoped>
.input {
  width: 382px;
  height: 21px;
  border-radius: 6px;
  border: solid 1px #DBE2EA;
  padding: 16px 0 15px 16px;
  outline-color: #0880AE;
}

.input::placeholder {
  color: #7C9CBF;
  font-size: 16px;
  font-weight: normal;
}

.input:active {
  border: solid 1px #DBE2EA;
}
</style>
