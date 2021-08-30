<template>
          <div
        class="test"
        style=""
      >
        <div class="d-flex flex-row align-start">
          <a
            href="https://www.google.co.th/?gws_rd=ssl"
            class="d-flex align-start text-decoration-none white--text font-weight-light"
            >รู้จัก TOCA ให้มากขึ้น</a
          >
          <span class="pl-2 pr-2 white--text">|</span>
          <a
            href="https://www.google.co.th/?gws_rd=ssl"
            class="d-flex align-start text-decoration-none white--text font-weight-light"
            >กระทู้ถาม - ตอบ</a
          >
          <span class="pl-2 pr-2 white--text">|</span>
          <a
            href="https://www.google.co.th/?gws_rd=ssl"
            class="d-flex align-start text-decoration-none white--text font-weight-light"
            >ปฎิทินกิจกรรม</a
          >
          <span class="pl-2 pr-2 white--text">|</span>
          <a
            href="https://www.google.co.th/?gws_rd=ssl"
            class="d-flex align-start text-decoration-none white--text font-weight-light"
            >กิจกรรมและสถานที่</a
          >
        </div>
        <div class="d-flex flex-row align-center">
          <a
            class="d-flex align-start text-decoration-none white--text font-weight-light"
            >สวัสดี {{ name }}</a
          >
          <img @click="open = !open" src="arrow.svg" alt="arrow" :class="open ? 'arrow-up' : 'arrow-down'" />
          <div>
            <span class="pl-1 pr-1 white--text">|</span>
          </div>
          <img :src="url.urlLink" class="pl-3" style="height:18px;" alt="test" />
          <span class="pl-2 pr-2 white--text">{{url.urlName}}</span>
        </div>
      </div>
</template>
<script>
export default {
  name: "App",
  data() {
    return {
      open: false,
      name: "Nat Srisawaivilai",
      url: {urlName: "EN", urlLink: "usFlag.svg",}
    };
  },
};

</script>

<style scoped>
  .arrow-down {
    height: 24px;
    transition: 0.5s;
  }

 .arrow-up {
   height: 24px;
    transition: 0.5s;
    transform: rotate(180deg);
  } 
  .test{
    width: 100vw; 
    height:100%; 
    max-height:30px; 
    padding:0 15vw;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
  @media screen {
    
  }
</style>