<template>
    <header class="bg-white">
            <nav class="navbar navbar-expand-lg bg-body-tertiary">
                <div class="container">
                    <a class="navbar-brand" href="#">C<img src="../assets/image/TitleIcon.png">VID19</a>
                    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
                      <span class="navbar-toggler-icon"></span>
                    </button>
                    <div class="collapse navbar-collapse positio-relative" id="navbarScroll">
                      <ul class="navbar-nav my-lg-0">
                        <li @click="hideMenu" class="nav-item  me-2">
                          <a class="nav-link active" aria-current="page" href="#">Home</a>
                        </li>
                        <li @click="hideMenu" class="nav-item me-2">
                          <a class="nav-link" href="#about">About Corona</a>
                        </li>
                        <li @click="hideMenu" class="nav-item me-2">
                          <a class="nav-link" href="#symptoms">Symptoms</a>
                        </li>
                        <li @click="hideMenu" class="nav-item me-2">
                          <a class="nav-link" href="#prevention">Prevention</a>
                        </li>
                        <li @click="hideMenu" class="nav-item  me-2">
                            <a class="nav-link" href="#treatment">Treatment</a>
                          </li>
                          <li @click="hideMenu" class="nav-item me-2">
                            <a class="nav-link" href="#question">FAQ</a>
                          </li>
                          <li @click="hideMenu" class="nav-item me-2">
                            <a class="nav-link" href="#latest">News</a>
                          </li>
                          <li @click="hideMenu" class="nav-item me-2">
                            <a href="#dont" class="nav-link btn btn-outline-primary text-light bg-primary rounded-5 ms-2">Do & Don't</a>
                          </li>
                      </ul>
                      <div @click="hideMenu" class="close position-absolute d-flex justify-content-center align-items-center text-white">
                        <i class="bi bi-x-circle-fill fs-1"></i>
                      </div>
                    </div>
                  </div>
              </nav>
    </header>
</template>

<style>
header{
    position: fixed;
    left: 0%;
    right: 0%;
    top: 0%;
    z-index: 99;
}
.navbar .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.navbar .container > a{
    font-weight: 900;
    color: var(--font-color);
    
}
.navbar .container > a >img {
    max-width: 30px;
    max-height: 30px;
}
.navbar .container > .collapse{
    width: 70%;
    justify-content: end !important;
}
.navbar .container > .collapse .navbar-nav  a{
    font-weight: bold;
}
.navbar .container > .collapse .navbar-nav  a:active,
.navbar .container > .collapse .navbar-nav  a:hover,
.active{
    color: var(--main-color) !important;
}
.navbar .container > .collapse .close{
  right: 20px;
  top: 20px;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background-color: #000;
  cursor: pointer;
  display: none;
  opacity: 0;
  z-index: -1;
}
@media (max-width: 991px) {
  .navbar .container{
    width: 100%;
  }
  .navbar .container > .collapse{
    background-color: #2d4062b1;
        min-height: 100vh;
        width: 100vw;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        margin: 0;
  }
  .navbar-nav{
    text-align: left;
    background-color: white;
    padding: 40px !important;
    height: 100%;
    max-width: 65%;
    position: absolute;
    top: 0;
    left: 0;
    justify-content: flex-start;
}
.navbar .container > .collapse .close{
  display: block;
  opacity: 1;
  z-index: 999;
}
}
</style>

<script>
export default{
  data(){

  },
  methods:{
    hideMenu:function(){
            let collapse = document.querySelector('.collapse')
            collapse.classList.remove('show')
        },
  },
}
</script>