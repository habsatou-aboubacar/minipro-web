<template>
  <div>
    <br />
    <div class="container">
      <div class="row">
        <div class="col">
          <form>
            <br />
            <h3>LOGIN</h3>
            <br />

            <div class="form-group">
              <label>Identifiant </label>
              <input type="email" class="form-control col-7" />
            </div>

            <div class="form-group">
              <label>Password</label>
              <input
                type="password"
                class="form-control form-control-lg col-7"
              />
            </div>

            <button type="submit" class="btn btn-dark btn-lg btn-block col-7">
              Sign In
            </button>

            <p class="forgot-password mt-2 mb-4">
              <router-link to="/forgot-password">Forgot password ?</router-link>
            </p>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.container {
    background-color:rgb(225, 232, 233)
}

</style>