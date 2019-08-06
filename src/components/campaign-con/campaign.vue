<template>
  <div class="container-fluid">
    <camHeader />
    <camBody :cam="[2, 0, 300, 300]" v-if="isApproved" @update-d="isApproved=false" />
    <camBodyItems :cam="[2, 0, 300, 300]" v-if="!isApproved" @update-d="isApproved=true" />
  </div>
</template>
<script>
import camHeader from "./camHeader";
import camBody from "./camBody";
import camBodyItems from "./camBodyItems";

export default {
  data() {
    return {
      isApproved: true
    };
  },
  components: {
    camHeader,
    camBody,
    camBodyItems
  }
};
</script>
<style>
</style>


