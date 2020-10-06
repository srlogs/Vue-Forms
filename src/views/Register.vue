<template>
  <div class="container">
    <h1>Registration Page</h1>
    <br />
    <br />
    <div class="row">
      <div class="col-md-3"></div>
      <div class="col-md-6">
        <form>
          <div class="form-group">
            <input
              type="text"
              class="form-control"
              id="username"
              placeholder="Enter your Username"
            />
          </div>
          <div class="form-group">
            <input
              type="email"
              class="form-control"
              id="exampleInputEmail1"
              placeholder="Enter your email"
              aria-describedby="emailHelp"
            />
          </div>

          <div class="form-group">
            <input
              type="password"
              class="form-control"
              placeholder="Enter your password"
              id="exampleInputPassword1"
            />
          </div>
          <button v-on:click="register" class="btn btn-primary">
            Register
          </button>
        </form>
      </div>
      <div class="col-md-3"></div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    register: function() {
        this.$router.push("/login");
    }
  }
};
</script>

<style scoped>
</style>