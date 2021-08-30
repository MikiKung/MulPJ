<template>
  <v-app>
    <div class="Nav">
      <UserNavbar />
    </div>
    <div>
      <SecondNavbar />
    </div>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import UserNavbar from "./components/allNavbar//UserNavbar.vue";
import SecondNavbar from "./components/allNavbar/SecondNavbar.vue";
export default {
  name: "App",
  components: { UserNavbar, SecondNavbar },
  data: () => ({
    name: "Nat Srisawaivilai ",
  }),
};
</script>
<style>
.Nav {
  display: flex;
  flex-direction: row;
  width: 100vw;
  background-color: #466430;
  position: fixed;
  z-index: 1000;
}
</style>
