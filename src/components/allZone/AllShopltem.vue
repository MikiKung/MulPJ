<template>
  <div class="Main">
    <div class="allShop">
      <div class="allHeadShop">
        <h1>สินค้าใหม่</h1>
      </div>
      <div class="mmm">
        <div :key="Index" v-for="(Item, Index) in Mockshop">
          <OneCard :Item="Item" :Index="Index"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import MockItem from "../../data/mockItem.json";
import OneCard from "../allZone/oneCard.vue";
export default {
  components: {
    OneCard,
  },
  computed: {
    Mockshop() {
      return MockItem.ShopItem.slice(0,5);
    },
  },
};
</script>

<style scoped>
.Main {
  padding: 20px 15vw;
  background-color: #eee;
}
.allShop {
  display: flex;
  flex-direction: column;
}
.allHeadShop {
  display: flex;
  justify-content: center;
}
.mmm{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
</style>
