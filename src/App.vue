<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light fixed-top mb-4 classA">
       <router-link to="/">
       <a class="navbar-brand font-weight-bold" href="#">
          <img src="@/assets/botgence.png" width="70" height="60" alt="">
          Botgence
         </a>
        </router-link>
        <button class="navbar-toggler bg-white" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon "></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav ml-auto p-2">
            <router-link to="/">
            <li class="nav-item active">
              <a class="nav-link text-white h6 font-weight-bold" href="#">HOME <span class="sr-only">(current)</span></a>
            </li>
            </router-link>
            <li class="nav-item dropdown">
                  <a class="nav-link dropdown-toggle h6 text-light font-weight-bold" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                    ABOUT US 
                  </a>
              <div class="dropdown-menu text-white" aria-labelledby="navbarDropdown">
                <router-link to="/about">
                  <a class="dropdown-item font-weight-bold" href="#">Our Story</a>
                </router-link>
                <router-link to="/technnology">
                  <a class="dropdown-item font-weight-bold" href="#">Technology</a>
                </router-link>
              </div>
            </li>
            <li class="nav-item">
              <router-link to="/blog">
              <a class="nav-link font-weight-bold h6 text-white" href="#">BLOG</a>
              </router-link>
            </li>
            <li class="nav-item">
              <router-link to="/products">
                <a class="nav-link font-weight-bold h6 text-white" href="#">PRODUCTS</a>
              </router-link>
            </li>
            <li class="nav-item">
              <router-link to="/contact">
                <a class="nav-link font-weight-bold h6 text-white" href="#">CONTACT</a>
              </router-link>
            </li>
             <li class="nav-item">
              <router-link to="">
                <a class="nav-link  text-primary" href="#">
                  <button class="my-btn btn-light h6 text-primary">GET A QOUTE</button>
                </a>
              </router-link>
            </li>
          </ul>
        </div>
    </nav>
    <router-view/>
  </div>
</template>

<style>
#app{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
  #nav a.router-link-exact-active {
    color: #42b983;
  }
  .classA{
    background-color:rgb(49, 156, 228);
    color: white;
  }
  a{
    font-family: Poppins;
  }
 .my-btn{
    border-radius: 30px 20px;
    width: 150px;
    border: 1px solid darkcyan;
  }
  .my-btn:hover{
    transform: translate3D(0,-40%,0);
    transition: all .8s;
  }
        
</style>


<script>
export default {
  name: 'App',
}

</script>

