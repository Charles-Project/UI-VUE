<template>
  <div class="container">
    <div class="campaign">
      <div class="row px-0">
        <div class="col-sm-6">
          <div
            class="d-flex flex-column justify-content-center campaign-title pl-1"
            v-on:click="cambodyOff"
          >
            <h4 class="mb-0">Convertproof</h4>
            <p class="mt-0">You have {{cam[0]}} CTA in this campaign</p>
          </div>
        </div>

        <div class="col-sm-5">
          <div class="d-flex justify-content-between py-sm-4 pr-1 pr-md-5 campaign-body">
            <div class="d-flex flex-column justify-content-center align-items-center">
              <h4 class="campaign-number mb-0 text-danger">{{cam[1]}}</h4>
              <p class="campaign-text text-secondary text-uppercase">views</p>
            </div>
            <div class="d-flex flex-column justify-content-center align-items-center">
              <h4 class="campaign-number mb-0 text-primary">{{ cam[2] }}</h4>
              <p class="campaign-text text-secondary text-uppercase">clicks</p>
            </div>
            <div class="d-flex flex-column justify-content-center align-items-center">
              <h4 class="campaign-number mb-0 text-success">{{cam[3]}}</h4>
              <p class="campaign-text text-secondary text-uppercase">leads</p>
            </div>
            <span class="d-flex justify-content-end">
              <i class="fa fa-ellipsis-h fas-absolute"></i>
            </span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["cam"],
  methods: {
    cambodyOff: function() {
      this.$emit("update-d", false);
    }
  }
};
</script>
<style scoped>
.campaign {
  background: #fff;
  margin-top: 1rem;
  padding-left: 2rem;
  font-family: "Roboto", sans-serif;
}

.campaign-title {
  margin-top: 2.2rem;
  cursor: pointer;
}

.campaign-title h4,
p {
  font-size: 0.9rem;
  font-weight: 500;
}

.campaign-title p {
  color: #b3becb;
}

.campaign-body {
  width: 100%;
}

.campaign-number {
  font-size: 2.3rem;
}

.campaign-text {
  font-size: 0.9rem;
  margin-top: 0;
}

/* font awesome */
span {
  position: absolute;
  top: 19%;
  right: -12%;
}

.fas-absolute {
  opacity: 0.2;
  font-size: 0.8rem;
}

/* media queries */
@media only screen and (max-width: 767px) {
  .campaign-number {
    font-size: 2rem;
  }

  .campaign-text {
    font-size: 0.8rem;
  }
}

@media only screen and (max-width: 578px) {
  body {
    overflow-x: hidden;
  }

  .campaign-title {
    margin-top: 1rem;
  }

  .campaign-number {
    font-size: 2rem;
  }

  .campaign-text {
    font-size: 0.8rem;
  }

  span {
    position: absolute;
    top: -69%;
    right: 7%;
  }
}
</style>



