<template>
  <div class="container-fluid px-0 my-3">
    <div class="milestone__container d-flex justify-content-between">
      <!-- milestone button and line -->
      <div class="milestone__entry">
        <div class="mentry__wrapper d-none d-sm-block">
          <h5 class="text-center">Milestone</h5>
          <div class="entry--text">Entry</div>
        </div>
        <div class="linecycle--wrapper">
          <div class="div--line"></div>
          <div class="div--cycle">1</div>
        </div>
      </div>
      <!-- milestone cards -->
      <div class="cardmilestone__container bg-white mr-0 mb-5 pb-3">
        <div class="title__wrapper">
          <h4 class="title">Title of Milestone</h4>
          <span class="awesome">
            <i class="fa fa-ellipsis-h fas-absolute"></i>
          </span>
        </div>
        <div class="d-sm-none d-flex mb-4 pl-2">
          <h5 class="text-center pr-3">Milestone</h5>
          <div class="div--entry">Entry</div>
        </div>
        <h5 class="h5--rewards">Rewards</h5>
        <div class="reward__items d-flex justify-content-between pl-0">
          <div class="row rewardCards">
            <EntryCard :items="items[1]" />
            <EntryCard :items="items[0]" />
            <EntryCard :items="items[1]" />
          </div>

          <div class="reward__container">
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
export default {
  components: {
    EntryCard
  },
  data: function() {
    return {
      items: [
        { id: 1, text: "400 points", color: "point--square" },
        { id: 2, text: "entry", color: "enter--radius" }
      ]
    };
  }
};
</script>
<style scoped>
.cardmilestone__container {
  padding-top: 9px;
  box-shadow: 5px 5px 10px 2px rgba(0, 0, 0, 0.13);
  flex: 1;
  padding: 5px 10px 1px 24px;
}

.awesome {
  position: absolute;
  top: 10%;
  left: 95%;
}

.title__wrapper {
  position: relative;
}

.milesTitle {
  font-size: 15px;
  margin-left: 9.6rem;
}

.milestone__entry {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 180px;
  position: relative;
  padding-left: 1rem;
}

.milestone__entry h5 {
  font-size: 17px;
  font-weight: 4;
}

.linecycle--wrapper {
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
}

.div--line {
  background-color: #e4e1e1;
  border-radius: 10px;
  height: 100%;
  position: absolute;
  width: 6px;
  top: -5px;
  left: 0;
}

.div--cycle {
  width: 41px;
  height: 41px;
  background: blue;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-size: 1.5rem;
  position: absolute;
  left: 0;
  top: 15px;
  transform: translateX(calc(-50% + 4px));
}

.mentry__wrapper {
  margin-top: 8px;
}

.mentry__wrapper h5 {
  margin-bottom: 4px;
}

.title {
  margin-top: 15px;
  margin-bottom: 3rem;
  margin-left: 9px;
  font-size: 1.7rem;
  color: #67758d;
}

.h5--rewards {
  text-transform: uppercase;
  margin-bottom: 1.1rem;
  font-size: 17px;
  color: #8c9db1;
}

/*  */
.div--entry {
  display: flex;
  padding: 0 20px;
  align-items: center;
  border: none;
  text-transform: uppercase;
  font-size: 13px;
  background-color: #e2e4ee;
  border-radius: 3px;
  font-weight: 500;
}

.entry--text {
  padding: 3px 26px;
  border: none;
  text-transform: uppercase;
  font-size: 13px;
  background-color: #e2e4ee;
  border-radius: 3px;
  font-weight: 500;
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

.rewardCards {
  width: 90%;
  border-right: 2px solid #f0f1f3;
}

.reward__container {
  width: 11%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.reward__container h5 {
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
}

@media (max-width: 871px) {
  .bttn-radius {
    left: 62%;
  }

  .bttn-square {
    left: 58%;
  }

  .reward__container h5 {
    font-size: 13px;
  }

  .btn-primary {
    width: 30px;
    height: 30px;
  }
}

@media (max-width: 822px) {
  .bttn-radius {
    padding: 1px 18px 3px 18px;
    border-radius: 20px;
    font-size: 10px;
  }
}

@media (max-width: 575px) {
  .milestone__entry {
    width: 10px;
  }

  .reward__container h5 {
    font-size: 10px;
  }

  .title {
    margin-bottom: 2rem;
  }
}

@media (max-width: 375px) {
  .title {
    font-size: 1.4rem;
  }
}
</style>

