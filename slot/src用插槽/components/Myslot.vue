<template>
  <span>
    <slot></slot>
  </span>
</template>

<script>
export default {};
</script>

<style>
.mydiv {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 15px;
  margin-left: 15px;
  width: 300px;
  height: 500px;
  background-color: burlywood;
}
.title {
  text-align: center;
  width: 100%;
  background-color: green;
}
</style>