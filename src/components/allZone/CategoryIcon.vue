<template>
  <div
    class="mb-10"
    style="display:flex; justify-content:center; padding-top:10px; width: 100%;"
  >
    <div
      style="width: 100%;"
      v-for="(Item, Index) in categories.category"
      :key="Index"
    >
      <router-link style="text-decoration:none;" :to="Item.Ilink" class="cateImage">
        <img :src="Item.Img" :alt="Item.name" />
        <span class="cateFont">{{ Item.name }}</span>
      </router-link>
    </div>
  </div>
</template>

<script>
import MockCategory from "../../data/mockCategory.json";
export default {
  computed: {
    categories() {
      return MockCategory;
    },
  },
};
</script>

<style>
.cateImage {
  border-left: 1px solid #afafaf;
  padding: 0 15px;
  height: 2rem;
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
}
.cateImage:last-child {
  border-right: 1px solid #afafaf;
}
.cateFont {
  font-family: "Courier New";
  font-size: 1px;
  font-weight: 600;
  display: flex;
  justify-content: end;
  padding-top: 5px;
  color: black;
  }
</style>
