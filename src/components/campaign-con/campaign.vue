<template>
  <div class="container-fluid">
    <camHeader />
    <camBody :cam="stat" />
  </div>
</template>
<script>
import camHeader from "./camHeader";
import camBody from "./camBody";

export default {
  components: {
    camHeader,
    camBody
  },
  data: function() {
    return {
      stat: [2, 0, 300, 300]
    };
  }
};
</script>
<style>
</style>


