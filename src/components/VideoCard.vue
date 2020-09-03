<template>
  <div class="video-card">
    <img class="thumbnail" :src="image" alt />
    <div class="video-info">
      <v-avatar size="30">
        <img :src="channelLogo" alt="Akash" />
      </v-avatar>
      <div class="video-text">
        <h4>{{title}}</h4>
        <p>{{channel}}</p>
        <p>{{views}} . {{timestamp}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VideoCard",
  props: ["image", "title", "channelLogo", "channel", "views", "timestamp"]
};
</script>

<style scoped>
.video-card {
  width: 240px;
  margin-bottom: 40px;
  margin-right: 20px;
}
.thumbnail {
  width: 246px;
  height: 138px;
}
.video-info {
  display: flex;
  margin-top: 10px;
  padding-right: 20px;
}
.video-text {
  margin-left: 10px;
  color: #030303eb;
}
h4 {
  margin-bottom: 5px;
}
p {
  color: #606060;
  font-size: 14px;
}
</style>