<template>
  <div class="Main ">
    <div class="mainGrid pt-5" style="width: 100%;">
      <div class="childgridOne mr-10">
        <div class="TopText">สมาคมผู้บริโภคอินทรีย์ไทย</div>
        <div class="TopText">Thai Organic Consumer Association</div>
        <div class="DataText">
          21 หมู่ 2 ถ.เพชรเกษม ต.ยายชา อ.สามพราน จ.นครปฐม 73310
        </div>
        <img style="height: 5rem; width: 100%;" src="NightLightTown.jpg" alt="Contacts" />
      </div>
      <!-- <v-divider inset vertical /> -->
      <div class="childgridTwo">
        <div class="childGrid">
          <div class="littleChildGrid">
            <div class="TopText">เกี่ยวกับสมาคมฯ</div>
            <router-link to="/home" class="linkText"
              ><div class="DataText">เกี่ยวกับเรา</div></router-link
            >
            <router-link to="/home" class="linkText"
              ><div class="DataText">ข่าวประชาสัมพันธ์</div></router-link
            >
            <router-link to="/home" class="linkText"
              ><div class="DataText">ปฎิทินกิจกรรม</div></router-link
            >
            <router-link to="/home" class="linkText"
              ><div class="DataText">กิจกรรมเเละสถานที่</div></router-link
            >
            <router-link to="/home" class="linkText"
              ><div class="DataText">สมัครสมาชิกสมาคมฯ</div></router-link
            >
            <router-link to="/home" class="linkText"
              ><div class="DataText">แผนผังเว็ปไซต์</div></router-link
            >
          </div>
          <div class="littleChildGrid">
            <div class="TopText">TOCA PLATFORM</div>
            <router-link to="/home" class="linkText"
              ><div class="DataText">ข้อมูลส่วนตัว</div></router-link
            >
            <router-link to="/home" class="linkText"
              ><div class="DataText">กระทู้ถาม/ตอบ</div></router-link
            >
          </div>
          <div class="littleChildGrid">
            <div class="TopText">ติดต่อเรา</div>
            <div class="DataText">
              เวลาทำการ: <span class="infoText2">test</span>
            </div>
            <div class="DataText">
              เวลา: <span class="infoText2">8.00 - 17.00 น.</span>
            </div>
            <div class="DataText">
              เบอร์โทรติดต่อ: <span class="infoText2">064-2954289</span>
            </div>
            <div class="DataText">
              อีเมล: <span class="infoText2">info.toca20@gmail.com</span>
            </div>
            <div class="DataText">
              Line Official Account:
              <span class="infoText2">@tocaplatform</span>
            </div>
          </div>
          <div class="littleChildGrid" style="margin:auto;">
            <img
              src="wink.jpg"
              alt="wink"
              class="mb-5"
              style="width: 120px; height: 120px; display:block;"
            />
            <img
              src="wink.jpg"
              alt="wink"
              style="width: 120px; height: 60px; display:block;"
            />
          </div>
        </div>
      </div>
    </div>

    <div>
      <span class="CopyRightText"
        >© Copy Right 2020 สมาคมผู้บริโภคอินทรีย์ไทย - Thai Organic Consumer
        Association</span
      >
    </div>
    <!-- <div class="d-flex flex-column pr-4">
            <span class="TopText">เกี่ยวกับสมาคม</span>
            <router-link to="/home" class="linkText"><span class="DataText">เกี่ยวกับเรา</span></router-link>
            <router-link to="/home" class="linkText"><span class="DataText">ข่าวประชาสัมพันธ์</span></router-link>
            <router-link to="/home" class="linkText"><span class="DataText">ปฎิทินกิจกรรม</span></router-link>
            <router-link to="/home" class="linkText"><span class="DataText">กิจกรรมเเละสถานที่</span></router-link>
            <router-link to="/home" class="linkText"><span class="DataText">สมัครสมาชิกสมาคมฯ</span></router-link>
            <router-link to="/home" class="linkText"><span class="DataText">แผนผังเว็ปไซต์</span></router-link>
        </div>
        <div  class="d-flex flex-column pr-4">
            <span class="TopText">TOCA PLATFORM</span>
            <router-link to="/home" class="linkText"><span class="DataText">ข้อมูลส่วนตัว</span></router-link>
            <router-link to="/home" class="linkText"><span class="DataText">กระทู้ถาม/ตอบ</span></router-link>
        </div>
        <div class="d-flex flex-column pr-4">
            <span class="TopText">ติดต่อเรา</span>
            <span class="DataText">เวลาทำการ: <span class="infoText2">test</span></span>
            <span class="DataText">เวลา: <span class="infoText2">8.00 - 17.00 น.</span></span>
            <span class="DataText">เบอร์โทรติดต่อ: <span class="infoText2">064-2954289</span></span>
            <span class="DataText">อีเมล: <span class="infoText2">info.toca20@gmail.com</span></span>
            <span class="DataText">Line Official Account: <span class="infoText2">@tocaplatform</span></span>
        </div>
        <div class="pr-4 d-flex flex-column ">
          <img src="wink.jpg" alt="wink" class="mb-2" style="width: 100px; height: 100px;">
          <img src="wink.jpg" alt="wink" style="width: 100px; height: 50px;">
        </div>
      </div>
    </div> -->

    <!-- 
        .CopyRightText {
      font-size: 12px;
      font-weight: 300;
      color: rgb(255, 255, 255);
    }
    .linkText{
      font-size:14px ;
      text-decoration: none !important;
      color: white !important;
    }
    .infoText1{
        font-size: 14px;
        color: #fff;
    }
    .infoText2{
        color: rgb(198, 198, 198);
    }
    .TopText{
      color: white;
      font-size: 12px;
      font-weight: 900;
    }
    .DataText{
      color: white;
      font-size: 10px;
    } -->
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.Main {
  display: flex;
  flex-direction: column;
  background-color: green;
  padding: 0 15vw;
}
.mainGrid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-gap: 1;
}
.childgridOne {
  grid-column: span 3;
}
.childgridTwo {
  grid-column: span 8;
}
.childGrid {
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  grid-gap: 50px;
}
.littleChildGrid {
  grid-column: span 2;
}
.TopText{
  color: #fff;
  font-size: 14px;
  font-weight: 700;
}
.DataText{
  color: #fff;
  font-size: 13px;
}
</style>
