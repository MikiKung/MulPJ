<template>
  <div
    style="width: 100%;  display: flex; flex-direction: row; justify-content: space-between;"
  >
    <div :key="Index" v-for="(Item, Index) in Mockshop">
        <OneCard :Item="Item" :Index="Index"/>
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
      return  MockItem.ShopItem.slice(0,4);
    },
  },
};
</script>

<style></style>
