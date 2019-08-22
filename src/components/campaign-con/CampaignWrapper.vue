<template>
  <div class="container-fluid">
    <CamHeader />
    <CamBody :stat="stat" />
  </div>
</template>
<script>
import CamHeader from "./CamHeader";
import CamBody from "./CamBody";

export default {
  components: {
    CamHeader,
    CamBody
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


