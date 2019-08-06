<template>
  <div class="container">
    <div class="apps-body bg-white px-4 pb-5">
      <div class="apps-header d-flex justify-content-between align-items-center pt-4 mb-2">
        <h2 class="brand-app">Your Apps</h2>
        <span class="toggle-app">
          <i class="fa fa-ellipsis-h fas-absolute"></i>
        </span>
      </div>

      <div class="available-apps px-3">
        <h5 class="mb-4">A List of Available Apps</h5>
        <!-- row 1 -->
        <div class="row mb-3">
          <!-- card 1 -->
          <div class="col-md-6 col-lg-4 mb-3">
            <div class="card card-app">
              <div class="card-body d-flex justify-content-between">
                <div class="app-header bg-dange">
                  <div class="app-icon">
                    <span>G</span>
                  </div>
                  <div class="app-body ml-2 pt-3">
                    <h5 class="mb-0">CTA</h5>
                    <p>Call to Action App</p>
                  </div>
                </div>
                <div class="app-button">
                  <label class="switch">
                    <input type="checkbox" checked />
                    <span class="slider round"></span>
                  </label>
                </div>
              </div>
            </div>
          </div>
          <!-- card 2 -->
          <div class="col-md-6 col-lg-4 mb-3">
            <div class="card card-app">
              <div class="card-body d-flex justify-content-between">
                <div class="app-header bg-dange">
                  <div class="app-icon">
                    <span>G</span>
                  </div>
                  <div class="app-body ml-2 pt-3">
                    <h5 class="mb-0">CTA</h5>
                    <p>Intuitive Analytic App</p>
                  </div>
                </div>
                <div class="app-button">
                  <label class="switch">
                    <input type="checkbox" checked />
                    <span class="slider round"></span>
                  </label>
                </div>
              </div>
            </div>
          </div>
          <!-- card 3 -->
          <div class="col-md-6 col-lg-4 mb-3">
            <div class="card card-app">
              <div class="card-body d-flex justify-content-between">
                <div class="app-header bg-dange">
                  <div class="app-icon">
                    <span>G</span>
                  </div>
                  <div class="app-body ml-2 pt-3">
                    <h5 class="mb-0">CTA</h5>
                    <p>Gamified lead Gen App</p>
                  </div>
                </div>
                <div class="app-button">
                  <label class="switch">
                    <input type="checkbox" checked />
                    <span class="slider round"></span>
                  </label>
                </div>
              </div>
            </div>
          </div>
          <!-- end -->
        </div>
        <!-- row 2 -->
        <div class="row mb-3">
          <!-- card 1 -->
          <div class="col-md-6 col-lg-4 mb-3">
            <div class="card card-app">
              <div class="card-body d-flex justify-content-between">
                <div class="app-header bg-dange">
                  <div class="app-icon">
                    <span>G</span>
                  </div>
                  <div class="app-body ml-2 pt-3">
                    <h5 class="mb-0">CTA</h5>
                    <p>Call to Action App</p>
                  </div>
                </div>
                <div class="app-button">
                  <label class="switch">
                    <input type="checkbox" checked />
                    <span class="slider round"></span>
                  </label>
                </div>
              </div>
            </div>
          </div>
          <!-- card 2 -->
          <div class="col-md-6 col-lg-4 mb-3">
            <div class="card card-app">
              <div class="card-body d-flex justify-content-between">
                <div class="app-header bg-dange">
                  <div class="app-icon">
                    <span>G</span>
                  </div>
                  <div class="app-body ml-2 pt-3">
                    <h5 class="mb-0">CTA</h5>
                    <p>Call to Action App</p>
                  </div>
                </div>
                <div class="app-button">
                  <label class="switch">
                    <input type="checkbox" checked />
                    <span class="slider round"></span>
                  </label>
                </div>
              </div>
            </div>
          </div>
          <!-- card 3 -->
          <div class="col-md-6 col-lg-4 mb-3">
            <div class="card card-app">
              <div class="card-body d-flex justify-content-between">
                <div class="app-header bg-dange">
                  <div class="app-icon">
                    <span>G</span>
                  </div>
                  <div class="app-body ml-2 pt-3">
                    <h5 class="mb-0">CTA</h5>
                    <p>Call to Action App</p>
                  </div>
                </div>
                <div class="app-button">
                  <label class="switch">
                    <input type="checkbox" checked />
                    <span class="slider round"></span>
                  </label>
                </div>
              </div>
            </div>
          </div>
          <!-- end -->
        </div>
        <!-- row 2 end -->
      </div>
    </div>
  </div>
</template>

<style>
.apps-header {
  opacity: 0.5;
}

.brand-app {
  font-size: 0.8rem;
  letter-spacing: 1px;
  text-transform: uppercase;
}

.toggle-app .fa {
  opacity: 0.5;
}

/*  */

.available-apps h5 {
  font-size: 0.9rem;
}

.app-header {
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.card-app {
  height: 130px;
}

.card-app .card-body {
  padding-top: 18px !important;
  padding-bottom: 18px !important;
}

.app-body {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.app-icon {
  width: 63px;
  height: 63px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #f2f4f7;
}

.app-body p {
  font-size: 14px;
  opacity: 0.5;
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
</style>

