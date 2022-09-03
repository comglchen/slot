<template>
  <div class="appdiv">
    <Myslot :categroy="phone" title="手机">this is replace myslot</Myslot>
    <Myslot :categroy="car" title="汽车">this is replace myslot</Myslot>
    <Myslot :categroy="food" title="食物">this is replace myslot</Myslot>
  </div>
</template>

<script>
import Myslot from "./components/Myslot";

export default {
  data() {
    return {
      phone: ["苹果", "华为", "三星"],
      car: ["福特", "奔驰", "宝马"],
      food: ["大白菜", "红萝卜", "西红柿"],
    };
  },
  components: {
    Myslot,
  },
};
</script>

<style>
.appdiv {
  display: flex;
  flex-direction: raw;
  margin: 15px;
}
</style>