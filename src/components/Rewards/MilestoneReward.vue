<template>
  <div class="container-fluid my-3">
    <div class="milestoneCon d-flex justify-content-between">
      <!-- milestone button and line -->
      <div class="milestoneEntry">
        <div class="mEntry">
          <h5>Milestone</h5>
          <button class="btnn btn-secondary" type="button">Entry</button>
        </div>
        <div class="lineCycle">
          <div class="mLine"></div>
          <div class="mCycle">1</div>
        </div>
      </div>
      <!-- milestone cards -->
      <div class="cardMilestone bg-white mr-0 mb-5 pb-3">
        <div class="titleMilesWrapper">
          <h4 class="titleMiles pl-4">Title of Milestone</h4>
          <span class="awesome">
            <i class="fa fa-ellipsis-h fas-absolute"></i>
          </span>
        </div>
        <h5 class="hh5">Rewards</h5>
        <div class="rewardItems d-flex justify-content-betweeen">
          <div class="row rewardCards">
            <EntryCard />
            <PointsCard />
          </div>
          <div class="rewardAdd">
            <button class="btn-primary">+</button>
            <h5>Add Reward</h5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import EntryCard from "./EntryCard";
import PointsCard from "./PointsCard";
export default {
  components: {
    EntryCard,
    PointsCard
  }
};
</script>
<style scoped>
.cardMilestone {
  padding-top: 9px;
  box-shadow: 5px 5px 10px 2px rgba(0, 0, 0, 0.13);
  flex: 1;
  padding: 5px 10px 1px 35px;
  /* position: relative; */
}

.awesome {
  position: absolute;
  top: 10%;
  left: 95%;
}

.titleMilesWrapper {
  position: relative;
}

.milesTitle {
  font-size: 15px;
  margin-left: 9.6rem;
}

.milestoneEntry {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 180px;
  position: relative;
}

.milestoneEntry h5 {
  font-size: 17px;
}

.lineCycle {
  position: absolute;
}

.mLine {
  position: absolute;
  width: 6px;
  background: #d3d8e6;
  height: 18rem;
  top: -5px;
  left: 89px;
  border-radius: 10px;
}

.mCycle {
  width: 48px;
  height: 48px;
  background: blue;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-size: 1.3rem;
  position: absolute;
  left: 67px;
  top: 15px;
}

.mEntry {
  margin-top: 16px;
}

.titleMiles {
  margin-top: 15px;
  margin-bottom: 3rem;
}

.hh5 {
  opacity: 0.5;
  text-transform: uppercase;
  margin-bottom: 1.1rem;
  font-size: 17px;
}

/*  */

.btnn {
  padding: 4px 25px;
  border: none;
  text-transform: uppercase;
}

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
}

.bttn-square {
  background: #ecedf1;
  color: black;
  font-size: 11px;
  padding: 3px 10px 4px 10px;
  font-weight: 500;
  position: absolute;
  top: 56%;
  left: 68%;
  border: none;
  text-transform: uppercase;
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

