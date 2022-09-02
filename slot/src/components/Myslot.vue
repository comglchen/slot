<template>
  <div>
    <div class="mydiv">
      <h1 class="title">{{ title }}</h1>
      <span v-for="(item, index) in categroy" :key="index">
        {{ item }}
      </span>
    </div>
  </div>
</template>

<script>
export default {
  props: ["categroy", "title"],
};
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
  background-color: yellow;
}
</style>