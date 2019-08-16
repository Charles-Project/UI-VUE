<template>
  <div class="container-fluid">
    <RewardNav />
    <MileStoneBtn />
    <MilestoneReward />
  </div>
</template>
<script>
import RewardNav from "./RewardNav";
import MileStoneBtn from "./MileStoneBtn";
import MilestoneReward from "./MilestoneReward";

export default {
  components: {
    RewardNav,
    MileStoneBtn,
    MilestoneReward
  },
  data: function() {
    return {
      images: [
        "https://image.shutterstock.com/image-photo/indoor-portrait-beautiful-brunette-young-600w-640005220.jpg",
        "https://www.shutterstock.com/image-photo/people-lifestyle-happiness-positive-human-expressions-682723735",
        "https://www.shutterstock.com/image-photo/woman-smiling-happiness-portrait-concept-520842832"
      ],
      title: [
        "title of milestone",
        "title of milestone2",
        "title of milestone3"
      ],
      rewardTitle: [
        "Reward title for the stuff",
        "Reward title for the stuff1"
      ],
      btnType: [
        { id: 1, color: "blue", text: "Entry" },
        { id: 2, color: "gray", text: "400 POINTS" }
      ]
    };
  }
};
</script>

<style scoped>
.container-fluid {
  background: #f4f6fc;
}
</style>
