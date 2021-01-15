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
              <label>Email address </label>
              <input type="email" class="form-control col-7" />
            </div>

            <div class="form-group">
              <label>Password</label>
              <input
                type="password"
                class="form-control form-control col-7"
              />
            </div>

            <button type="submit" class="btn btn-dark btn-lg btn-block col-7" @click="auth">
              Sign In
            </button>
            <!-- <button type="button" id="get-joke" >
              Get a Joke!!
            </button> -->
            {{ result }}
            <p class="forgot-password mt-2 mb-4">
              <router-link to="/forgot-password">Forgot password ?</router-link>
            </p>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
.container {
  background-color: rgb(225, 232, 233);
}
</style>
<script>
import axios from 'axios';

export default {
  data: function(){
    return {
      result:{},
      responseAvailable: false
    };
    
  },
  methods: {
    auth(){
      axios.get("https://jsonplaceholder.typicode.com/todos/1")
      .then(response => response.json())
      // .then(json => console.log(json))
      .then(response => (this.result = response));
    },
    fetchAPIData() {
      this.responseAvailable = false;
      fetch(
        "http://127.0.0.1/PrTp/Users/Users.php?Email=non.massa.nonQuisquefringilla.org&Password=162906135401",
        {
          mode: 'no-cors',
          method: "GET",
          headers: { },
        }
      )
        .then((response) => {
          console.log("---LLLL ",response);
          return response.json();
          // if (response.ok) {
          //   return response.json();
          // } else {
          //   alert(
          //     "Server returned " + response.status + " : " + response.statusText
          //   );
          // }
        })
        .then((response) => {
          console.log("---",response.status);
          // this.result = response.body;
          // alert(this.result)
          // this.responseAvailable = true;
        })
        .catch((err) => {
          console.log(err);
        });
    },
  },
};
</script>
