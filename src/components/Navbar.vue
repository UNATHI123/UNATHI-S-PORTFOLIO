<template >
  <header id="header" class="fixed-top d-flex align-items-cente">
<div class="container-fluid container-xl d-flex align-items-center justify-content-lg-between">   
<nav class="navbar navbar-expand-lg navbar-light bg-light-sticky-top">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">UNATHI QOLWENI</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
           <a class="nav-link scrollto " href="#hero">HOME</a>
          <a class="nav-link scrollto" href="#about">ABOUT</a>
          <a class="nav-link scrollto" href="#skills">SKILLS</a>
          <a class="nav-link scrollto" href="#resume">RESUME</a>
          <a class="nav-link scrollto" href="#projects">PROJECTS</a>
          <a class="nav-link scrollto" href="#testimonials">TESTIMONIALS</a>
          <a class="nav-link scrollto" href="#contact">CONTACT</a>
         </div>
    </div>
  </div>
</nav>
    </div>
  
    
  </header>
</template>
<script>

  
</script>
<style scoped>
#header {
  background:#37332a;
  border-bottom: 1px solid rgba(12, 11, 9, 0.6);
  transition: all 0.5s;
  z-index: 997;
  padding: 15px 0;
  top: 40px;
}

#header.header-scrolled {
  top: 0;
  background:black;
  border-bottom: 1px solid ;
}
#header .logo {
  font-size: 28px;
  margin: 0;
  padding: 0;
  line-height: 1;
  font-weight: 300;
  letter-spacing: 1px;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
}


.navbar-light .navbar-nav .nav-link {
    color: white;
}
.navbar-light .navbar-brand {
    color: lightseagreen;
}
.navbar-light .navbar-nav .nav-link :hover {
    color: lightseagreen;
    
}
</style>
