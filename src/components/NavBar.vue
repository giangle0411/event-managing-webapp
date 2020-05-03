<template>
  <div id="nav" class="nav">
    <v-app-bar app color="#39b982">
      <v-btn text to="/">Real World Events</v-btn>
      <v-spacer></v-spacer>
      <v-btn text :to="{ name: 'event-list' }"> List</v-btn>
      <v-btn text :to="{ name: 'event-create' }">Create</v-btn>
    </v-app-bar>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
}
.nav > .brand {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  font-size: 1.5em;
  color: #39b982;
  text-decoration: none;
}
.nav .nav-item {
  box-sizing: border-box;
  margin: 0 10px;
  color: rgba(0, 0, 0, 0.5);
  text-decoration: none;
}
.nav .nav-item.router-link-exact-active {
  color: #39b982;
  border-bottom: solid 2px #39b982;
}
</style>
