<template>
  <div class="shopCard">
    <div class="DetialCard">
      <div class="shopRecommand">
        <span class="recommandText">เเนะนำ</span>
        <div>
          <img
            @click="switches"
            style="height:15px; margin-right:5px;"
            :src="fillHeart[test]"
            alt="heart"
          />
        </div>
      </div>
      <img class="itemShop" :src="Item.sImg" :alt="Item.sId" />
    </div>
    <div style="padding-left:10px; padding-right:10px">
      <div style=" height:50px;">
        <div class="shopHeadText"> {{Item.sName}} </div>
        <div class="shopDetailText">
          {{ truncate(Item.sDetail, 25, "...") }}
        </div>
      </div>
      <div>
        <span class="shopETCText">
        {{  truncate(Item.sLocation, 28, "...") }}
        </span>
      </div>
      <div class="priceAndQuan pt-2">
        <span class="shopPriceText"> ฿ {{Item.sPrice}}  </span>
        <span class="shopETCText">
          {{ Item.sQuantity }}
        </span>
      </div>
      <router-link to="/home" style="text-decoration:none;">
        <div class="buying mt-1 py-2">
          <img style="height: 16px;" src="shopping_cart.svg" alt="cart" />
          <span class="buyingText">หยิบใส่ตะกร้า</span>
        </div>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
    props:{
        Item:Object,
        Index:Number
    },
  methods: {
    truncate(text, length, suffix) {
      if (text.length > length) {
        return text.substring(0, length) + suffix;
      } else {
        return text;
      }
    },
    switches() {
      this.test = (this.test + 1 )%2 ;
    },
  },
  data() {
    return {
      fillHeart: ["blank_heart.svg", "fill_heart.svg"],
      test: 0,
    };
  },
};
</script>

<style>
.shopCard {
  width: 170px;
  height: 100%;
  background-color: rgb(243, 240, 240);
  border-radius: 10px;
  padding-bottom: 10px;
}
.itemShop {
  border-top-right-radius: 10px;
  border-top-left-radius: 10px;
  object-fit: cover;
  height: 150px;
  width: 100%;
}
.shopRecommand {
  position: absolute;
  margin-top: 10px;
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: space-between;
}
.recommandText {
  padding: 5px 13px;
  font-weight: bold;
  font-size: 10px;
  border-radius: 3px;
  background-color: rgb(223, 231, 57);
}
.DetialCard {
  position: relative;
}
.shopHeadText {
  font-size: 12px;
  font-weight: bold;
}
.shopDetailText {
  font-size: 9px;
  color: rgb(113, 113, 113);
}
.shopPriceText {
  font-size: 15px;
  font-weight: lighter;
  color: red;
}
.shopETCText {
  font-size: 9px;
}
.priceAndQuan {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.buying {
  display: flex;
  flex-direction: row;
  justify-content: center;
  background-color: rgb(202, 202, 202);
  border-radius: 5px;
  align-items: center;
  cursor: pointer;
}
.buyingText {
  color: white;
  font-size: 12px;
  cursor: pointer;
}
</style>
