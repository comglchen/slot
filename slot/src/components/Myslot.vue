<template>
  <span>
    <slot :food="food" :car="car" :phone="phone"></slot>
  </span>
</template>

<script>
export default {
  data() {
    return {
      phone: ["苹果", "华为", "三星"],
      car: ["福特", "奔驰", "宝马"],
      food: ["大白菜", "红萝卜", "西红柿"],
    };
  },
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
  background-color: green;
}
</style>