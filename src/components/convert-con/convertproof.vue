<template>
  <div class="container-fluid pb-4 mt-4">
    <convertCard />
    <convertitem />
  </div>
</template>
<script>
import convertCard from "./convertCard";
import convertitem from './convertitems'
export default {
  components: {
    convertCard,
    convertitem
  }
};
</script>

