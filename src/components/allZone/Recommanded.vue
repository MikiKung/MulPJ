<template>
  <div class="recomm">
    <div
      style="padding-right:160px; display:flex; flex-direction: column; justify-content:center;"
    >
      <h3 class="whiteTHText" style="cursor:default;">สินค้าเเนะนำ</h3>
      <h3 class="whiteENText" style="cursor:default;">Recommanded</h3>
      <router-link to="/home" class="moreItemText"><i>ดูสินค้าเเนะนำทั้งหมด ></i></router-link>
    </div>
      <CardItem />
  </div>
</template>

<script>
import CardItem from "../allZone/CardItem.vue";
export default {
  components: {
    CardItem,
  },
};
</script>

<style>
.recomm {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 2rem 15vw;
  background-image: url("/wink.jpg");
  background-position: top;
  background-size: cover;
  width: 100%;
  height: auto;
}
.recomCardRow{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.moreItemText{
  font-size:8px ;
  text-decoration: none !important;
  color: white !important;
}
.whiteTHText{
  color: white;
  font-size: 22px;
}
.whiteENText{
  color: white;
}
</style>
