<template>
  <v-contianer>
    <div style="display:flex; flex-direction:row; flex-wrap:wrap;">
      <div class="testGrid">
        <img src="wink.jpg" alt="wink" class="cardPoster" />
      </div>
      <div class="test2">
        <div>
          <img src="wink.jpg" style="width: 100%;  object-fit: cover; height:8.25rem; border-radius: 10px; display:block;" alt="wink" />
        </div>
        <div>
          <img src="wink.jpg" style="width: 325px; object-fit: cover; height: 8.25rem;  border-radius: 10px; display:block;" alt="wink" />
        </div>
      </div>
  <div>
    <div>
      
    </div>
  </div>
    </div>
  </v-contianer>
</template>

<script>
export default {
  name: "PosterCard",
};
</script>

<style>
.cardPoster {
  width: 45rem;
  height: 17rem;
  border-radius: 10px;
  object-fit: cover;
}
.testGrid {
  display: grid;
}
.test2{
   display:flex; 
   flex-direction: column;
   justify-content: space-between;
   padding-left:10px;
  }
</style>
