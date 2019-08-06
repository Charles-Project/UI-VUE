<template>
  <div class="container mt-5" id="app">
    <div class="campaign1-header d-flex justify-content-between align-items-center mb-4">
      <div class="campaign1-cta pl-md-4">
        <div class="campaign1-icon d-flex align-items-center mb-2">
          <span class="ctapp-brand mr-3">G</span>
          <h4>CTA APP</h4>
        </div>
        <h1 class="campaign1-text text-uppercase">Campaigns</h1>
      </div>
      <button type="button" class="btn btn-primary add-campaign">Add Campaign</button>
    </div>
  </div>
</template>

<script>
</script>
<style scoped>
/* -------------- campaign header---------------- */

.ctapp-brand {
  width: 47px;
  height: 47px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background: skyblue;
}

.campaign1-icon h4 {
  opacity: 0.7;
}

.campaign1-text {
  font-size: 2.2rem;
  opacity: 0.8;
}

.add-campaign {
  opacity: 0.4;
  padding: 11px 60px;
}

/* -----------------    media queries    ----------------------------- */

@media (max-width: 991px) {
}

@media (max-width: 767px) {
  .campaign1-header {
    display: flex;
    flex-direction: column;
    align-items: start !important;
  }

  .campaign1-text {
    font-size: 2rem;
  }
}
</style>

