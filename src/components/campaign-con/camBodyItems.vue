<template>
  <!-- ------ convert proof 1 header ------ -->
  <div class="container">
    <div id="cvtproof">
      <div class="cvtproof d-flex justify-content-between py-4 px-4">
        <div class="cvtproof-brand d-flex align-items-center">
          <span class="cvtproof-icon mr-1 mr-sm-4">
            <i class="fas fa-caret-left"></i>
          </span>
          <div class="cnvtproof-text">
            <h6 class="text-uppercase txt-h6">Convertproof</h6>
            <h6>Configure CTA Widgets</h6>
          </div>
        </div>
        <div class="cvtproof-widget d-flex">
          <button type="button" class="btn btn-primary btn-sm mr-sm-3 mr-0">Add Widgets</button>
          <span class="cvtproof__fa pt-2">
            <i class="fa fa-ellipsis-h"></i>
          </span>
        </div>
      </div>
      <!--  -->
      <div class="status-container bg-white">
        <div class="status-page">
          <div class="row pl-4">
            <div class="col-md-6">
              <div class="status-icon d-flex pt-3">
                <p class="text-uppercase mr-3">status</p>
                <div>
                  <label class="switch">
                    <input type="checkbox" checked />
                    <span class="slider round"></span>
                  </label>
                </div>
              </div>
              <h4>Buy page</h4>
            </div>
            <div class="col-md-6 pr-lg-5">
              <div class="d-flex justify-content-between py-sm-2 pr-3 pr-md-5 campaign-body">
                <div class="d-flex flex-column justify-content-center align-items-center">
                  <h4 class="status-number mb-1 text-danger">{{cam[1]}}</h4>
                  <p class="status-text text-secondary text-uppercase">views</p>
                </div>
                <div class="d-flex flex-column justify-content-center align-items-center">
                  <h4 class="status-number mb-1 text-primary">{{cam[2]}}</h4>
                  <p class="status-text text-secondary text-uppercase">clicks</p>
                </div>
                <div class="d-flex flex-column justify-content-center align-items-center">
                  <h4 class="status-number mb-1 text-bright">{{cam[3]}}</h4>
                  <p class="status-text text-secondary text-uppercase">leads</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["cam"]
};
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
  font-size: 3rem;
  opacity: 0.8;
}

.add-campaign {
  opacity: 0.4;
  padding: 11px 60px;
}

/* ----------- converproof header --------------- */

.cvtproof {
  background: #f7f9ff;
}

.cvtproof-icon {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background: white;
}

.cnvtproof-text h6:nth-child(1) {
  font-size: 0.9rem;
  opacity: 0.6;
}

.cvtproof-icon .fas {
  color: #0029dc;
  font-size: 1.8rem;
}

.cvtproof-widget button {
  padding: 9px 66px;
}

/* .cvtproof__fa {
  position: absolute;
  top: 40%;
  left: 93%;
  transform: translate(-50%, -50%);
} */

.cvtproof__fa .fa {
  opacity: 0.3;
  font-size: 0.8rem;
}

/* ------------------------- -- campaign status -- ------------------------------- */
.status-page {
  border: 1px solid #e0e7ff;
  border-radius: 5px;
}

.status-container {
  padding: 2rem 3rem;
}

.status-icon p {
  opacity: 0.7;
  margin-block-end: 0;
  font-size: 0.8rem;
}

.status-page h4 {
  opacity: 0.8;
  font-size: 1.2rem;
}

/* slider style */
.switch {
  position: relative;
  display: inline-block;
  width: 34px;
  height: 18px;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 15px;
  width: 15px;
  left: 0;
  bottom: 2px;
  background-color: white;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

input:checked + .slider {
  background-color: #33ac2e;
}

input:focus + .slider {
  box-shadow: 0 0 1px #33ac2e;
}

input:checked + .slider:before {
  -webkit-transform: translateX(17px);
  -ms-transform: translateX(17px);
  transform: translateX(17px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 36px;
}

.slider.round:before {
  border-radius: 50%;
}
/* slyder style end */

.text-bright {
  color: #7aebf7;
}

.status-title h4,
p {
  font-size: 0.9rem;
  font-weight: 500;
}

.status-title p {
  color: #b3becb;
}

.status-body {
  width: 100%;
}

.status-number {
  font-size: 2.5rem !important;
}

.status-text {
  font-size: 0.9rem;
  margin-top: 0;
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

  .cvtproof-widget button {
    padding: 0px 10px;
    font-size: 8px;
    line-height: 1;
  }
}

@media (max-width: 576px) {
  .cvtproof-widget {
    display: flex;
    flex-direction: column;
  }
  .cvtproof-widget button {
    order: 2;
    padding: 8px 10px;
    font-size: 10px;
  }

  .cvtproof__fa .fa {
    display: flex;
    justify-content: flex-end;
    padding-top: 0px;
  }
}

@media (max-width: 450px) {
  .cvtproof-icon {
    width: 30px;
    height: 30px;
  }

  .cnvtproof-text h6 {
    font-size: 0.7rem;
  }

  .cvtproof-icon .fas {
    font-size: 1.4rem;
  }

  .txt-h6 {
    font-size: 0.8rem !important;
  }

  .status-container {
    padding: 2rem 1rem;
  }
}
</style>

