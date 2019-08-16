<template>
  <div class="container-fluid">
    <div class="row">
      <VisitCard :points="points" />
      <VisitCard :points="points" />
      <VisitCard :points="points" />
    </div>
  </div>
</template>
<script>
import VisitCard from "./VisitCard";
export default {
  components: {
    VisitCard
  },
  data: function() {
    return {
      points: "500"
    };
  }
};
</script>
<style scoped>
</style>