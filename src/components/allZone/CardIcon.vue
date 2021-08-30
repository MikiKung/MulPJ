<template>
  <div class="greyCard">
      <div :key="Index" v-for="(Item, Index) in mockCard.card">
        <div class="greyInCard">
          <img class="greyImg" :src="Item.cImg" :key="Index" :alt="Index" />
          <span class="greyText">{{ Item.cName }}</span>
        </div>
      </div>
    </div>
</template>

<script>
import MockCard from "../../data/mockCard";
export default {
  computed: {
    mockCard() {
      return MockCard;
    },
  },
};
</script>

<style>
.greyCard {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100%;
  background-color: #eee;
  padding:35px 15vw;
}
.greyInCard {
  display: flex;
  flex-direction: column;
  position: relative;
}
.greyImg {
  width: 14rem;
  height: 6rem;
  border-radius: 20px;
}
.greyText {
  border-radius: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  position: absolute;
  font-size: 16px;
  color: #fff;
  background-color: rgba(0, 0, 0, 0.5);
}
</style>
