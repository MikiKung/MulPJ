<template>
      <div
      class="SecondNavbar mt-6 white darken-3 d-flex justify-space-between align-center w-sm-8"
    >
      <img src="wink.jpg" alt="wink"  class="LogoWeb" />
      <div
        class="d-flex diraction-column"
        style="border-bottom:2px solid green"
      >
        <input
          type="text"
          placeholder="ค้นหาสินค้า"
          
          style=" width: 400px; outline:none;"
        />
        <button class="d-flex align-center">
          <img
            style="transform: rotate(270deg);"
            src="arrow-green.svg"
            alt="arrow"
          />
        </button>
      </div>
      <div class="d-flex flex-nowrap" >
        <button>
          <div class="d-flex align-center">
            <img src="arrow-black.svg" alt="arrow" />
            <span>สินค้าทั้งหมด</span>
          </div>
        </button>
        <button>
          <div class="d-flex align-center">
            <img src="arrow-black.svg" alt="arrow" />
            <span>สินค้าทั้งหมด</span>
          </div>
        </button>
      </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
::placeholder {
  color: rgba(85, 171, 87, 1);
}
.SecondNavbar{
  box-shadow:0px 12px 7px 0px #f5f5f5; 
  width: 100%; 
  padding:0 15vw;
}
.LogoWeb{
  height:60px; 
  width: 200px; 
  object-fit: cover;
}

@media screen and (max-width: 1264px){

}
</style>