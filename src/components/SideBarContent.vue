<template>
  <div
    :class="[
      'sidebar-content',
      selected ? 'sidebar-content-selected' : null,
    ]"
  >
    <v-icon class="icon" size="25">{{icon}}</v-icon>
    <h6 class="title">{{title}}</h6>
  </div>
</template>

<script>
export default {
  name: "SideBarContent",
  props: ["title", "icon", "selected"]
};
</script>

<style scoped>
.sidebar-content {
  display: flex;
  align-items: center;
  padding: 10px 20px;
}
.sidebar-content:hover {
  background: lightgray;
  cursor: pointer;
}
.sidebar-content-selected {
  background: lightgray;
  cursor: pointer;
}
.sidebar-content-selected > .icon {
  color: red;
}
.sidebar-content-selected > .title {
  font-weight: bold;
}
.title {
  margin-left: 20px;
  font-weight: 400;
  font-size: 14px;
}
</style>