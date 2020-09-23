<template>
  <v-container style="height:100%">
        <Appbar/>
<Navigationbar/>
<Home/>
<Chatnavigation/>
  </v-container>
</template>

<script>
import Appbar from "../components/Appbar";
import Navigationbar from "../components/Navigationbar";
import Home from "../components/Home";
import Chatnavigation from "../components/Chatnavigation";


export default {
  data() {
    return {
    };
  },
  components:{
    Appbar,
    Navigationbar,
    Home
  }
};
</script>

<style>
</style>