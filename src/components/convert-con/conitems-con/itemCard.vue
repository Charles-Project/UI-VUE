<template>
  <div class="col-md-6 col-lg-4 mb-3">
    <div class="card card-app">
      <div class="card-body d-flex justify-content-between">
        <div class="app-header bg-dange">
          <div class="app-icon">
            <span>G</span>
          </div>
          <div class="app-body ml-2 pt-3">
            <h5 class="mb-0">{{ctaH}}</h5>
            <p>{{ctaP}}</p>
          </div>
        </div>
        <div class="app-button">
          <label class="switch" @change="changeUpdate">
            <input type="checkbox" checked />
            <span class="slider round"></span>
          </label>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["ctaH", "ctaP"],
  methods: {
    changeUpdate: function() {
      this.$emit("update:switch");
    }
  }
};
</script>

