<template >
    
  <!-- ======= Hero Section ======= -->
  <section id="hero" class="d-flex align-items-center">
    <div class="container position-relative text-center text-lg-start" data-aos="zoom-in" data-aos-delay="100">
      
      <div class="row">
        <div class="col-lg-8">
          <h1><span>UNATHI QOLWENI</span></h1>
<div class="typewriter">
  <h2>ASPIRING WEB DEVELOPER</h2>
</div><br><br>
<div class="social-icons">
  <a class="social-icon social-icon--codepen" href="https://codepen.io/unathi123" target="_blank">
    <i class="fa fa-codepen"></i>
    <div class="tooltip">Codepen</div>
  </a>
  <a class="social-icon social-icon--github" href="https://github.com/UNATHI123" target="_bllank">
    <i class="fa fa-github"></i>
    <div class="tooltip">Github</div>
  </a>
  <a class="social-icon social-icon--linkedin" href="https://www.linkedin.com/in/unathi-qolweni-3584a0224/" target="_blank">
    <i class="fa fa-linkedin"></i>
    <div class="tooltip">LinkedIn</div>
  </a>

</div>
          <div class="btns">
            <a href="#about" class="btn-menu animated fadeInUp scrollto">ABOUT ME</a>
            <a href="#contact" class="btn-book animated fadeInUp scrollto">CONTACT </a>
          </div>
        </div>
        

      </div>
    </div>
  </section>
  <!-- End Hero -->


</template>
<script>
export default {
  
}
</script>
<style scoped >
    #hero {
  width: 100%;
  height: 100vh;
  background: url(https://images.pexels.com/photos/2512387/pexels-photo-2512387.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1) top center;
  background-size: cover;
  position: relative;
  padding: 0;
}
#hero:before {
  content: "";
  /* background: rgba(0, 0, 0, 0.5); */
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
}
#hero .container {
  padding-top: 110px;
}
@media (max-width: 992px) {
  #hero .container {
    padding-top: 98px;
  }
}
#hero h1 {
  margin: 0;
  font-size: 48px;
  font-weight: 700;
  line-height: 56px;
  color: #fff;
  font-family: "Poppins", sans-serif;
}
#hero h1 span {
  color:black;
}

#hero .btns {
  margin-top: 30px;
}
#hero .btn-menu, #hero .btn-book {
  font-weight: 600;
  font-size: 13px;
  letter-spacing: 0.5px;
  text-transform: uppercase;
  display: inline-block;
  padding: 12px 30px;
  border-radius: 50px;
  transition: 0.3s;
  line-height: 1;
  color: black;
  border: 2px solid black;
}
#hero .btn-menu:hover, #hero .btn-book:hover {
  background: lightseagreen;
  color: black;
}
#hero .btn-book {
  margin-left: 15px;
}
#hero .play-btn {
  width: 94px;
  height: 94px;
  background: radial-gradient(#cda45e 50%, rgba(205, 164, 94, 0.4) 52%);
  border-radius: 50%;
  display: block;
  position: relative;
  overflow: hidden;
}
#hero .play-btn::after {
  content: "";
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translateX(-40%) translateY(-50%);
  width: 0;
  height: 0;
  border-top: 10px solid transparent;
  border-bottom: 10px solid transparent;
  border-left: 15px solid #fff;
  z-index: 100;
  transition: all 400ms cubic-bezier(0.55, 0.055, 0.675, 0.19);
}
#hero .play-btn::before {
  content: "";
  position: absolute;
  width: 120px;
  height: 120px;
  -webkit-animation-delay: 0s;
  animation-delay: 0s;
  -webkit-animation: pulsate-btn 2s;
  animation: pulsate-btn 2s;
  -webkit-animation-direction: forwards;
  animation-direction: forwards;
  -webkit-animation-iteration-count: infinite;
  animation-iteration-count: infinite;
  -webkit-animation-timing-function: steps;
  animation-timing-function: steps;
  opacity: 1;
  border-radius: 50%;
  border: 5px solid rgba(205, 164, 94, 0.7);
  top: -15%;
  left: -15%;
  background: rgba(198, 16, 0, 0);
}
#hero .play-btn:hover::after {
  border-left: 15px solid #cda45e;
  transform: scale(20);
}
#hero .play-btn:hover::before {
  content: "";
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translateX(-40%) translateY(-50%);
  width: 0;
  height: 0;
  border: none;
  border-top: 10px solid transparent;
  border-bottom: 10px solid transparent;
  border-left: 15px solid #fff;
  z-index: 200;
  -webkit-animation: none;
  animation: none;
  border-radius: 0;
}
@media (min-width: 1024px) {
  #hero {
    background-attachment: fixed;
  }
}
@media (max-width: 992px) {
  #hero .play-btn {
    margin-top: 30px;
  }
}
@media (max-height: 500px) {
  #hero {
    height: auto;
  }
  #hero .container {
    padding-top: 130px;
    padding-bottom: 60px;
  }
}
@media (max-width: 768px) {
  #hero h1 {
    font-size: 28px;
    line-height: 36px;
  }
  #hero h2 {
    font-size: 18px;
    line-height: 24px;
  }
}

@-webkit-keyframes pulsate-btn {
  0% {
    transform: scale(0.6, 0.6);
    opacity: 1;
  }
  100% {
    transform: scale(1, 1);
    opacity: 0;
  }
}

@keyframes pulsate-btn {
  0% {
    transform: scale(0.6, 0.6);
    opacity: 1;
  }
  100% {
    transform: scale(1, 1);
    opacity: 0;
  }
}

.typewriter h2 {
  color: black !important;
  font-family: monospace;
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  /* border-right: .15em solid orange; The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  letter-spacing: .15em; /* Adjust as needed */
  animation: 
    typing 3.5s steps(30, end),
    blink-caret .5s step-end infinite;
}

/* The typing effect */
@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

/* The typewriter cursor effect */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: orange }
}
.social-icons {
  display: flex;
}

.social-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  width: 80px;
  height: 80px;
  margin: 0 0.5rem;
  border-radius: 50%;
  cursor: pointer;
  font-family: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
  font-size: 2.5rem;
  text-decoration: none;
  transition: all 0.15s ease;
}
.social-icon:hover {
  color: #fff;
}
.social-icon:hover .tooltip {
  visibility: visible;
  opacity: 1;
  transform: translate(-50%, -150%);
}
.social-icon:active {
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.5) inset;
}
.social-icon--linkedin {
  background: #006599;
  color: #fff;
}
.social-icon--linkedin .tooltip {
  background: #006599;
  color: currentColor;
}
.social-icon--linkedin .tooltip:after {
  border-top-color: #006599;
}
.social-icon--codepen {
  background: #000;
  color: #fff;
}
.social-icon--codepen .tooltip {
  background: #000;
  color: currentColor;
}
.social-icon--codepen .tooltip:after {
  border-top-color: #000;
}
.social-icon--github {
  background: #4284c0;
  color: #fff;
}
.social-icon--github .tooltip {
  background: #4284c0;
  color: currentColor;
}
.social-icon--github .tooltip:after {
  border-top-color: #4284c0;
}
.social-icon i {
  position: relative;
  top: 1px;
}

/* Tooltips */
.tooltip {
  display: block;
  position: absolute;
  top: 0;
  left: 50%;
  padding: 0.8rem 1rem;
  border-radius: 40px;
  font-size: 0.8rem;
  font-weight: bold;
  opacity: 0;
  pointer-events: none;
  text-transform: uppercase;
  transform: translate(-50%, -100%);
  transition: all 0.3s ease;
  z-index: 1;
}
.tooltip:after {
  display: block;
  position: absolute;
  bottom: 1px;
  left: 50%;
  width: 0;
  height: 0;
  content: "";
  border: solid;
  border-width: 10px 10px 0 10px;
  border-color: transparent;
  transform: translate(-50%, 100%);
}
</style>