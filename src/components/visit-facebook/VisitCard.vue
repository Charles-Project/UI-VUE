<template>
  <div class="col-sm-6 col-lg-4 mb-5">
    <div class="card">
      <div class="card-main">
        <div>
          <h3 class="text-capitalize">Visit us on facebook</h3>
        </div>
        <div class="card-icons">
          <div class="card-edit">
            <i class="fas fa-pen"></i>
            <div>edit</div>
          </div>
          <div class="card-duplicate">
            <i class="far fa-clone"></i>
            <div>duplicate</div>
          </div>
          <div class="card-delete">
            <i class="far fa-trash-alt"></i>
            <div>delete</div>
          </div>
        </div>
      </div>
      <div class="card-pointer">
        <div class="card-line"></div>
        <div class="card-points">
          <h4 class="text-primary text-center">{{points}}</h4>
          <h5 class="text-uppercase text-center">Points</h5>
        </div>
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
  flex: 1;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  padding-top: 10px;
  padding-bottom: 10px;
}
.card-main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 75%;
}

.card-main h3 {
  font-size: 1.2rem;
  color: #7a879b;
  margin-bottom: 0.5rem;
}
.card-icons {
  display: flex;
  justify-content: space-between;
  background: #f8f8f8;
}

.card-duplicate,
.card-delete,
.card-edit {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 5px 8px;
}

.card-duplicate div,
.card-delete div,
.card-edit div {
  font-size: 12px;
  font-weight: 500;
}

.card-duplicate i,
.card-delete i,
.card-edit i {
  padding-right: 3px;
  font-size: 11px;
}

.card-pointer {
  display: flex;
  width: 25%;
}

.card-line {
  width: 3%;
  background: #e0e2e8;
  height: 80px;
}
.card-points {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 96%;
}

.card-points h4 {
  font-size: 1.7rem;
  font-weight: 500;
  margin-bottom: 0;
  text-align: center;
}

.card-points h5 {
  font-size: 1rem;
  font-weight: 500;
  text-align: center;
}

/* media */
@media (max-width: 1145px) {
  .card-main h3 {
    font-size: 1rem;
  }

  .card-duplicate div,
  .card-delete div,
  .card-edit div {
    font-size: 10px;
    font-weight: 500;
  }

  .card-duplicate i,
  .card-delete i,
  .card-edit i {
    padding-right: 2px;
    font-size: 9px;
  }
}

@media (max-width: 991px) {
  .card-main h3 {
    font-size: 1.2rem;
  }
}

@media (max-width: 774px) {
  .card-main h3 {
    font-size: 0.9rem;
  }

  .card-points h4 {
    font-size: 1.15rem;
  }

  .card-points h5 {
    font-size: 0.8rem;
  }
}

@media (max-width: 687px) {
  .card-main h3 {
    font-size: 0.9rem;
  }

  .card-points h4 {
    font-size: 1.15rem;
  }

  .card-points h5 {
    font-size: 0.8rem;
  }
}

@media (max-width: 576px) {
  .card-main h3 {
    font-size: 1.2rem;
  }

  .card-duplicate div,
  .card-delete div,
  .card-edit div {
    font-size: 12px;
  }

  .card-duplicate i,
  .card-delete i,
  .card-edit i {
    padding-right: 3px;
    font-size: 11px;
  }

  .card-points h4 {
    font-size: 1.7rem;
  }

  .card-points h5 {
    font-size: 1rem;
  }
}

/* @media (max-width: 454px) {
  .card-main h3 {
    font-size: 0.9rem;
  }

  .card-points h4 {
    font-size: 1.15rem;
  }

  .card-points h5 {
    font-size: 0.8rem;
  }
} */
</style>
