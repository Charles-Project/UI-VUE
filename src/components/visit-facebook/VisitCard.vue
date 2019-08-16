<template>
  <div class="col-md-6 col-lg-4 mr-0 my-3">
    <div class="card d-flex justify-content-between flex-row">
      <div class="card-main">
        <h3>Visit Us on Facebook</h3>
        <div class="card-icons d-flex justify-content-between">
          <div class="card-edit">
            <p>edit</p>
            <i class="fas fa-pen"></i>
          </div>`
          <div class="card-duplicate">
            <p>duplicate</p>
            <i class="far fa-clone"></i>
          </div>
          <div class="card-delete">
            <p>delete</p>
            <i class="far fa-trash-alt"></i>
          </div>
        </div>
      </div>
      <div class="line-div"></div>
      <div class="card-points">
        <h3>{{points}}</h3>
        <h5 class="text-uppercase">Points</h5>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["points"]
};
</script>
<style scoped>
.card {
  display: flex;
  width: 25rem;
  padding: 0.5rem 0.5rem 0.5rem 3rem;
  position: relative;
}

.card-main {
  opacity: 0.7;
  display: flex;
  justify-content: center;
  flex-direction: column;
  width: 65%;
  margin-top: 10px;
}

.card-main div {
  background: #f8f8f8;
  padding: 0 5px;
}

.card-main div .card-edit,
.card-delete,
.card-duplicate {
  display: flex;
  align-items: center;
}

.card-main p {
  order: 2;
  margin-left: 3px;
  margin-top: 14px;
}

.card-main h3 {
  text-align: center;
}

.card-main .far,
.fas {
  font-size: 10px;
}

.card-main h3 {
  font-size: 1.3rem;
}

.card-points {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.card-points h3 {
  color: #304cff;
  font-size: 1.5rem;
  margin-bottom: 0;
}

.card-points h5 {
  font-size: 1.2rem;
}

.line-div {
  height: 90px;
  width: 3px;
  background: #e0e2e8;
  position: absolute;
  left: 77%;
}
</style>