<template>
  <div>
    <CampaignWrapper />
    <graphic />
    <convertproof />
    <RewardCon />
    <VisitFacebook />
  </div>
</template>

<script>
import CampaignWrapper from "./components/campaign-con/CampaignWrapper";
import graphic from "./components/graphic-con/graphic";
import convertproof from "./components/convert-con/convertproof";
import RewardCon from "./components/Rewards/RewardCon";
import VisitFacebook from "./components/visit-facebook/VisitFacebook";
export default {
  name: "app",
  components: {
    CampaignWrapper,
    graphic,
    convertproof,
    RewardCon,
    VisitFacebook
  }
};
</script>

<style>
</style>
