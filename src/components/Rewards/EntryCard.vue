<template>
  <div class="col-md-6 col-lg-4 mb-4">
    <div class="card d-flex flex-row justify-content-start">
      <div class="card-img"></div>
      <div class="card--main ml-1">
        <h5>Reward Title for the stuff</h5>
        <div :class="items.color">{{items.text}}</div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    items: Object
  }
};
</script>
<style scoped>
.card {
  padding: 12px 0 12px 10px;
  border-radius: 10px;
  flex: 1;
}

.card-img {
  width: 50px;
  height: 50px;
  background: yellow;
  border-radius: 50%;
}

.card--main {
  flex: 1;
  padding-right: 10px;
}

.card--main h5 {
  font-size: 14px;
  margin-left: 7px;
  margin-bottom: 14px;
  color: #c1cad5;
}

.enter--radius {
  width: 75px;
  border-radius: 20px;
  background: #2da6ba;
  color: whitesmoke;
  font-size: 12px;
  padding: 3px 0;
  border: none;
  text-align: center;
  text-transform: uppercase;
  cursor: none;
  margin-left: auto;
}

.point--square {
  background: #ecedf1;
  width: 80px;
  text-align: center;
  color: black;
  font-size: 12px;
  padding: 3px 0;
  font-weight: 500;
  border: none;
  text-transform: uppercase;
  margin-left: auto;
}

/* media queries */
@media (max-width: 1250px) {
  .card-img {
    width: 45px;
    height: 45px;
  }

  .card h5 {
    font-size: 12px;
  }
}

@media (max-width: 991px) {
  .card-img {
    width: 50px;
    height: 50px;
  }

  .card h5 {
    font-size: 14px;
  }
}

@media (max-width: 871px) {
  .point--square {
    left: 58%;
  }
}
</style>