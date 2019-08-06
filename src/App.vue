<template>
  <div>
    <campaign />
    <graphic />
    <convertproof />
  </div>
</template>

<script>
import campaign from "./components/campaign-con/campaign";
import graphic from "./components/graphic-con/graphic";
import convertproof from "./components/convert-con/convertproof";
export default {
  name: "app",
  components: {
    campaign,
    graphic,
    convertproof
  }
};
</script>

<style>
</style>
