<template>
<!--<head>
  <div class="bg-dark">
    <div class="container">
      <div class="row">
        <nav class="col navbar navbar-expand-lg navbar-dark">
          <a class="navbar-brand" href="/">
            <img
              src="images/elac_logo.png"
              width="50"
              height="50"
              alt="Info Logo"
            />
            Info School
          </a>
          <button
            class="navbar-toggler"
            type="button"
            data-toggle="collapse"
            data-target="#navbarContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div id="navbarContent" class="collapse navbar-collapse">
            <ul class="navbar-nav">
              <li class="nav-item active">
                <a class="nav-link" href="/">Accueil</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="/">Cours</a>
              </li>
              <li class="nav-item"></li>
              <a class="nav-link" href="/Connecter">login</a>
            </ul>
          </div>
        </nav>
        <div>
          <b-navbar type="light" variant="light">
            <b-nav-form>
              <b-form-input class="mr-sm-2" placeholder="Search"></b-form-input>
              <b-button
                variant="outline-success"
                class="my-2 my-sm-0"
                type="submit"
                >Search</b-button
              >
            </b-nav-form>
          </b-navbar>
          
        </div>
      </div>
    </div>
  </div>
</head>!-->
  <div>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="/Debut">
      <img src="../assets/elac_logo.png" width="40" height="30" alt="Site logo">
      
       Karatu
       </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
       <b-navbar-nav>
        <b-nav-item active href ="/Debut">Home</b-nav-item>
      </b-navbar-nav>
      <b-navbar-nav>
        <b-nav-item active href ="/">Cours</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
        </b-nav-form>

        <!--pour les regrouper <b-nav-item-dropdown right>-->
          <!-- Using 'button-content' slot -->
          <template #button-content>
            <!--<em>User</em>-->
          </template> 
          <router-link to="/Connecter">
          <b-dropdown-item  href="/Connecter">
           login 
          </b-dropdown-item>
          </router-link>
          
          <b-dropdown-item  href="/signup">Register</b-dropdown-item>
          
          <router-link to="/CPF">
          <b-dropdown-item  href="/CPF">login professeur</b-dropdown-item>
           </router-link>
       <!-- </b-nav-item-dropdown>-->
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>
<script>
export default {};
</script>