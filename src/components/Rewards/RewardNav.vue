<template>
  <div class="row">
    <div class="col-2"></div>
    <div class="col-10">
      <ul class="nav d-flex justify-content-center">
        <li class="nav-item pl-3">
          <a class="nav-link active" href="#">Details</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-secondary" href="#">Milestones</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-secondary" href="#">Design</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-secondary" href="#">Advanced</a>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.row {
  border-top: 1px solid #dddee3;
  background: white;
}
.nav-item {
}
a {
  font-weight: 500;
  padding: 2rem 2rem 0.2rem 2rem;
}

.active {
  color: blue;
  background: #eaeeff;
  border-bottom: 3px solid blue;
}
</style>


