<template>
  <div class="appdiv">
    <span class="mydiv"
      ><h1 class="cate">手机分类</h1>
      <Myslot v-for="(d, index) in phone" :key="index">{{ d }}</Myslot>
    </span>
    <span class="mydiv"
      ><h1 class="cate">汽车分类</h1>
      <Myslot v-for="(d, index) in car" :key="index">{{ d }}</Myslot>
    </span>
    <span class="mydiv"
      ><h1 class="cate">食物分类</h1>
      <Myslot v-for="(d, index) in food" :key="index">{{ d }}</Myslot>
    </span>
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
.appdiv {
  display: flex;
  flex-direction: raw;
  margin: 15px;
}
.cate {
  text-align: center;
  width: 100%;
  background-color: rgb(197, 194, 23);
}
</style>