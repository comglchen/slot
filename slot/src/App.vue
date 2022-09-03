<template>
  <div class="appdiv">
    <myslot>
      <template scope="{food}">
        <span class="mydiv">
          <h1 class="cate">食物分类</h1>
          <span v-for="(f, index) in food" :key="index">{{ f }}</span>
        </span>
      </template>
    </myslot>
    <myslot>
      <template scope="{car}">
        <span class="mydiv">
          <h1 class="cate">汽车分类</h1>
          <span v-for="(c, index) in car" :key="index">{{ c }}</span>
        </span>
      </template>
    </myslot>
    <myslot>
      <template scope="{phone}">
        <span class="mydiv">
          <h1 class="cate">手机分类</h1>
          <span v-for="(p, index) in phone" :key="index">{{ p }}</span>
        </span>
      </template>
    </myslot>
  </div>
</template>


 

<script>
import Myslot from "./components/Myslot";

export default {
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