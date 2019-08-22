<template>
  <div class="d-flex justify-content-between py-sm-2 pr-3 pr-md-5 campaign-body">
    <div class="d-flex flex-column justify-content-center align-items-center">
      <h4 class="status-number mb-1 text-danger">{{stat[1]}}</h4>
      <p class="status-text text-secondary text-uppercase">views</p>
    </div>
    <div class="d-flex flex-column justify-content-center align-items-center">
      <h4 class="status-number mb-1 text-primary">{{stat[2]}}</h4>
      <p class="status-text text-secondary text-uppercase">clicks</p>
    </div>
    <div class="d-flex flex-column justify-content-center align-items-center">
      <h4 class="status-number mb-1 text-bright">{{stat[3]}}</h4>
      <p class="status-text text-secondary text-uppercase">leads</p>
    </div>
  </div>
</template>
<script>
export default {
  props: ["stat"]
};
</script>

