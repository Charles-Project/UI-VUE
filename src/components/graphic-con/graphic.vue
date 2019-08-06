<template>
  <div>
    <div class="container bg-white mt-3 py-4">
      <div class="row pl-3 pr-1">
        <div class="col-10 d-flex col-sm-10">
          <span class="graphic-icon mr-3 d-flex justify-content-center align-items-center">G</span>
          <div class="graphic-title d-flex flex-column justify-content-center pl-0">
            <h5>graphics</h5>
            <h5>Design beautiful banners easily</h5>
          </div>
        </div>

        <div class="col-2 d-flex justify-content-end">
          <div class="graphics-toggle">
            <i class="fa fa-ellipsis-h"></i>
          </div>
        </div>
      </div>
    </div>

    <div class="container mt-5">
      <div class="row add-website d-flex justify-content-center align-items-center">
        <button class="btn">Add Website</button>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.graphic-icon {
  height: 67px;
  width: 67px;
  background: #f2f4f7;
  border-radius: 50%;
  font-size: 1.8rem;
}

.graphic-title h5 {
  font-size: 0.9rem;
  text-transform: capitalize;
}

.graphic-title h5:nth-child(1) {
  margin-bottom: 0;
  margin-bottom: 1px;
}
.graphic-title h5:nth-child(2) {
  color: #b0bbc9;
}

.graphics-toggle .fa {
  margin-top: 1rem;
  opacity: 0.3;
  cursor: pointer;
}

/* --------- add website ------------------- */
.add-website {
  border: 2px dotted #2e5bff;
  border-radius: 5px;
  padding: 2.5rem 0;
}

.btn {
  background: transparent;
  outline: none;
  border: none;
  cursor: pointer;
  opacity: 0.5;
  text-transform: uppercase;
}
/* --------------------  */

/* media queries */
@media only screen and (max-width: 450px) {
  .graphic-icon {
    height: 58px;
    width: 58px;
    font-size: 1.6rem;
  }

  .graphic-title h5 {
    font-size: 0.6rem;
  }
}
</style>



