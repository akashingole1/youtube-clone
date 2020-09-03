<template>
  <div class="sidebar">
    <SideBarContent v-bind:selected="selected" icon="home" title="Home" />
    <SideBarContent icon="whatshot" title="Trending" />
    <SideBarContent icon="subscriptions" title="Subscriptions" />
    <div class="line"></div>
    <SideBarContent icon="video_library" title="Library" />
    <SideBarContent icon="history" title="History" />
    <SideBarContent icon="slideshow" title="Your videos" />
    <SideBarContent icon="watch_later" title="Watch later" />
    <SideBarContent icon="thumb_up_alt" title="Liked videos" />
  </div>
</template>

<script>
import SideBarContent from "./SideBarContent";

export default {
  name: "SideBar",
  components: {
    SideBarContent
  },
  data() {
    return {
      selected: true
    };
  }
};
</script>

<style scoped>
.sidebar {
  flex: 2;
  color: black;
}
.line {
  height: 1px;
  border-bottom: 1px solid lightgray;
  margin: 10px 0px;
}
</style>