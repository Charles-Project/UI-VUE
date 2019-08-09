<template>
  <div class="container-fluid pb-4 mt-4">
    <convertCard />
    <convertitem />
  </div>
</template>
<script>
import convertCard from "./card-con/convertCard";
import convertitem from "./conitems-con/convertitems";
export default {
  components: {
    convertCard,
    convertitem
  }
};
</script>

