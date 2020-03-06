<template>
  <div id="Navbar">
    <div class="row nav-div">
      <img class="col s2" src="../assets/images/fide-logo.svg" alt="logo">
      <h1 class="col s10">International Chess Federation</h1>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Navbar',
}
</script>

<style lang="scss" scoped>

$color: #334166;

#Navbar {
  background: $color;
  color: white;
}

.nav-div {
  padding: 15px;
}

h1 {
  font-size: 24px;
}

</style>