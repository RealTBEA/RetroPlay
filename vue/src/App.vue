<template>
  <div id="main">
    <div id="nav">
      <NavBar></NavBar>
    </div>
    <!-- <div id="app">
      <router-link v-bind:to="{ name: 'home' }">Home</router-link>&nbsp;|&nbsp;
      <router-link v-bind:to="{ name: 'logout' }" v-if="$store.state.token != ''">Logout</router-link>
    </div> -->
    <div id="routerview">
      <router-view />
    </div>
  </div>

</template>

<script>
import NavBar from "./components/Nav"; 
export default {
  components: {NavBar}
};
</script>

<style>

body {
  background-color: #000022;
  background-image: url("/recordbackground.png");
  background-attachment: fixed;
  background-repeat: no-repeat;
  color: aliceblue;
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
}

.app {
  background-color: greenyellow;
}

#routerview {
  align-items: center;
  top: 100px;
  width: 98%;
  margin-top: 110px;

}

#recordbackground {
  align-items: center;
  align-self: center;
  bottom: 0px;
}

</style>