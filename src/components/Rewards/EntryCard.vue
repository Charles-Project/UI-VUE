<template>
  <div class="col-md-6 col-lg-4 mb-4">
    <div class="card d-flex flex-row justify-content-start">
      <div class="card-img"></div>
      <h5>Reward Title for the stuff</h5>
      <button class="bttn bttn-radius">entry</button>
    </div>
  </div>
</template>
<style scoped>
.card {
  padding: 12px 0 12px 10px;
  border-radius: 10px;
  flex: 1;
  position: relative;
}

.card-img {
  width: 50px;
  height: 50px;
  background: yellow;
  border-radius: 50%;
}

.card h5 {
  font-size: 14px;
  margin-left: 7px;
  color: #c1cad5;
}

.bttn-radius {
  border-radius: 20px;
  background: #2da6ba;
  color: whitesmoke;
  font-size: 12px;
  padding: 2px 20px 4px 20px;
  position: absolute;
  top: 56%;
  left: 70%;
  border: none;
  text-transform: uppercase;
  cursor: none;
}

/* ----------- rewards item div for the cards and add rewards ------------------------- */
/*  */

/*  */
.rewardItems {
  position: relative;
}

.rewardCards {
  width: 92%;
  border-right: 2px solid #f0f1f3;
  padding-right: 14px;
}

.rewardAdd {
  position: absolute;
  right: -7px;
  top: -1px;
  /* border-left: 2px solid #f0f1f3; */
  width: 99px;
  padding-left: 10px;
  padding-right: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.rewardAdd h5 {
  font-size: 15px;
  text-align: center;
}

.btn-primary {
  border-radius: 50%;
  border: none;
  width: 40px;
  height: 40px;
  margin-bottom: 10px;
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

  .bttn-radius {
    top: 58%;
    left: 65%;
    padding: 1px 18px 3px 18px;
    border-radius: 20px;
    font-size: 11px;
  }

  .bttn-square {
    font-size: 10px;
    padding: 3px 10px 4px 10px;
    left: 62%;
  }
}

@media (max-width: 1098px) {
  .bttn-radius {
    left: 61%;
  }

  .bttn-square {
    left: 58%;
  }

  .rewardAdd {
    right: -15px;
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

  .bttn-radius {
    top: 58%;
    left: 66%;
    padding: 2px 20px 4px 20px;
    border-radius: 20px;
    font-size: 12px;
  }

  .bttn-square {
    left: 65%;
  }

  .mLine {
    height: 24rem;
    top: -5px;
    left: 89px;
    border-radius: 10px;
  }
}

@media (max-width: 871px) {
  .bttn-radius {
    left: 62%;
  }

  .bttn-square {
    left: 58%;
  }

  .rewardAdd {
    width: 79px;
  }

  .rewardAdd h5 {
    font-size: 13px;
  }

  .btn-primary {
    width: 30px;
    height: 30px;
  }
}

@media (max-width: 822px) {
  .bttn-radius {
    /* top: 58%;
    left: 65%; */
    padding: 1px 18px 3px 18px;
    border-radius: 20px;
    font-size: 10px;
  }
}
</style>