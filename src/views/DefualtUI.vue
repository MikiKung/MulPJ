<template>
  <div>
    <div class="Outer">
      <poster-card />
      <category-icon />
    </div>
    <div>
      <card-icon />
      <recommanded/>
      <all-shop-item/>
      <img-zone/>
      <contact-us/>
    </div>
  </div>
</template>

<script>
import PosterCard from "../components/allZone/PosterCard.vue";
import CategoryIcon from "../components/allZone/CategoryIcon.vue";
import CardIcon from "../components/allZone/CardIcon.vue";
import Recommanded from "../components/allZone/Recommanded.vue";
import AllShopItem from "../components/allZone/AllShopltem.vue";
import ImgZone from "../components/allZone/ImgZone.vue";
import ContactUs from "../components/allZone/contactUs.vue";

export default {
  name: "DefualtUI",
  components: {
    PosterCard,
    CategoryIcon,
    CardIcon,
    Recommanded,
    AllShopItem,
    ImgZone,
    ContactUs
  },
};
</script>

<style>
.Outer {
  display: flex;
  justify-content: space-between;
  padding: 20px 15vw;
  flex-wrap: wrap;
}
</style>
