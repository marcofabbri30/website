<template>
    <header>
        <nav class="navbar fixed-top navbar-light bg-transparent px-3" id="header-bar">

            <div class="container d-flex flex-wrap ">
                <a class="navbar-brand" href="#" id="testId">
                    <img src="../assets/logo_prw.png" width="35" height="35" alt=""> 
                    Marco Fabbri</a>
                <!-- <div class="d-none d-md-block"> -->
                <div>
                    <ul class="nav ">
                        <li class="nav-item"><a href="#heroSection" class="nav-link">Home</a></li>
                        <li class="nav-item"><a href="#aboutMeSection" class="nav-link">About me</a></li>
                        <li class="nav-item"><a href="#servicesSection" class="nav-link">Services</a></li>
                    </ul>
                </div>
                <!-- <div class="d-md-none">
                    <button class="hamburger hamburger--3dx" :class="{'is-active':hamburgerIsActive}" type="button" v-on:click="hamburgerIsActive = !hamburgerIsActive">
                        <span class="hamburger-box">
                            <span class="hamburger-inner"></span>
                        </span>
                    </button>
                </div> -->
                                
            <!--  -->
            </div>
        <!-- <RouterLink to="/">Home</RouterLink> -->
        </nav>
    </header>

</template>

<style>

/* aside {
    display: flex;
    flex-direction: column;
    width: 100%;
    min-height:100vh;
    overflow:hidden;
    padding:1rem;
    transition: 0.2s ease-out;
} */

#header-bar{
  transition: background-color 100ms linear; 
}
#header-bar .navbar-brand{
  color:white
}

.nav-link{
    color: grey !important
}
.active {
    color:white !important
}
/* .test{
  color: black !important
} */

</style>

<script>
export default{
    data(){
        return {
            hamburgerIsActive: false
        }
    }
}
var hamburger = document.querySelector(".hamburger");

window.onscroll = function() {myFunction()};

// bg-light

// hamburger.addEventListener("click", function() {
//     debugger;
//     // Toggle class "is-active"
//     hamburger
//     // Do something else, like open/close menu
// });

function myFunction() {
  if (document.body.scrollTop > 50 || document.documentElement.scrollTop > 50) {
    document.getElementById("header-bar").classList.remove("bg-transparent");
    document.getElementById("header-bar").classList.add("bg-dark");
    // document.getElementById("testId").classList.add("test");
  } else {
    document.getElementById("header-bar").classList.remove("bg-dark");
    document.getElementById("header-bar").classList.add("bg-transparent");
    // document.getElementById("testId").classList.remove("test");
  }
}

//   // Look for .hamburger
//   // On click

</script>