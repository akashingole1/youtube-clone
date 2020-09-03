<template>
  <div class="header">
    <div class="logo-section">
      <v-icon class="icon" size="25">menu</v-icon>
      <img class="logo" src="../assets/images/logo2.webp" alt="YouTube" />
    </div>
    <div class="input-section">
      <input placeholder="Search" type="text" />
      <v-icon class="search" size="25">search</v-icon>
    </div>
    <div class="header-icons">
      <v-icon class="icon" size="25">video_call</v-icon>
      <v-icon class="icon" size="25">apps</v-icon>
      <v-icon class="icon" size="25">notifications</v-icon>
      <v-avatar size="30">
        <img
          src="https://avatars2.githubusercontent.com/u/31619784?s=460&u=d578bdb981c9604a2350cc06182387097071f818&v=4"
          alt="Akash"
        />
      </v-avatar>
    </div>
  </div>
</template>

<script>
// import logo from "../assets/images/logo1.jpg";
export default {
  name: "Header"
};
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px 20px;
  position: sticky;
  top: 0;
  z-index: 1;
  background: white;
  margin-bottom: 10px;
}
.logo-section {
  display: flex;
  align-items: center;
}
.logo {
  height: 27px;
  /* margin-left: 20px; */
}
.input-section {
  display: flex;
  align-items: center;
  border: 1px solid lightgray;
  width: 40%;
}
.input-section > input {
  flex: 1;
  border: none;
  padding-left: 10px;
  font-size: 16px;
  padding-top: 4px;
  padding-bottom: 4px;
}

input[type="text"]:focus {
  outline: none;
}

.header-icons {
  display: flex;
  align-items: center;
}
.search {
  background: #f8f8f8;
  width: 50px;
  color: gray;
}
.icon {
  margin-right: 15px;
}
</style>