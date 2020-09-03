<template>
  <div>
    <!-- Header -->
    <Header />
    <div class="content">
      <SideBar />
      <VideoSection />
    </div>
  </div>
  <!-- <v-app>
    <v-main>
      <Header />
    </v-main>
  </v-app>-->
</template>

<script>
import Header from "./components/Header";
import SideBar from "./components/SideBar";
import VideoSection from "./components/VideoSection";

export default {
  name: "App",

  components: {
    Header,
    SideBar,
    VideoSection
  },

  data: () => ({
    //
  })
};
</script>

<style scoped>
.content {
  display: flex;
}
</style>
