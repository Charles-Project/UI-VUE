<template>
  <div class="card">
    <div class="card-body d-flex justify-content-between align-items-center" :class="bgcolor">
      <div class="card-icon" :class="iconBg">
        <i class="far" :class="icon"></i>
      </div>
      <div class="card-text">
        <h3>{{cardtextH}}</h3>
        <p>{{cardtextP}}</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["bgcolor", "icon", "iconBg", "cardtextP", "cardtextH"]
};
</script>
<style scoped>
</style>


