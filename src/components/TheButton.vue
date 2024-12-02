<template>
  <button class="button"><slot></slot></button>
</template>

<script>
export default {
  name: "TheButton",
};
</script>

<style scoped>
.button {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 8px 10px;
  border: none;
  border-radius: 5px;
  background-color: #282828;
  color: #639eff;
  cursor: pointer;
}
</style>
