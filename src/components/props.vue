<template>
  <div class="backdrop">
    <div class="modal">
      <h1>{{ header }}</h1>
      <p>{{ text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["header", "text"],
};
</script>

<style scoped>
.modal {
  width: 200px;
  padding: 20px;
  margin: 50px auto;
  background: red;
  border-radius: 10px;
}
.backdrop {
  top: 0;
  position: fixed;
  background: rgba(0, 0, 0, 0.5);
  width: 100%;
  height: 100%;
}
h1 {
  color: #03cfb4;
  border: none;
  padding: 0;
}
</style>
