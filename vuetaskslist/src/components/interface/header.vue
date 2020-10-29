<template>
  <div>
    <div>
      <b-navbar type="dark" variant="dark">
        <b-navbar-nav>
          <b-nav-item to="/">
            <img src="../../assets/logo.png" class="logo" />
          </b-nav-item>
          <b-navbar-brand to="/">VueTasks</b-navbar-brand>
          <b-nav-item to="/">Home</b-nav-item>
          <b-nav-item to="/about">About</b-nav-item>
        </b-navbar-nav>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.logo {
  width: 25px;
}
</style>
