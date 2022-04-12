<template>
<Navbar />
<Home />
<About />
<Skills />
<Resume />
<Projects />
<Testimonials />
<Contact />
<Footer />


</template>

<script>
import  Navbar from './components/Navbar.vue'
import  Home from './components/Home.vue'
import  About from './components/About.vue'
import  Skills from './components/Skills.vue'
import Resume from './components/Resume.vue'
import Projects from './components/Projects.vue'
import Testimonials from './components/Testimonials.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'



export default {

  components: {
    Navbar,
    Home,
    About,
    Skills,
    Resume,
    Projects,
    Testimonials,
    Contact,
    Footer

  }
}
</script>
 <style>
#app {
  font-family: "Open Sans", sans-serif;
  background:#fff;
  color:#000;
}

h1, h2, h3, h4, h5, h6 {
  font-family: "Playfair Display", serif;
  font-weight: bold
}
section {
  padding: 60px 0;
  overflow: hidden;
}



.section-title {
  padding-bottom: 40px;
}
.section-title h2 {
  font-size: 14px;
  font-weight: 500;
  padding: 0;
  line-height: 1px;
  margin: 0 0 5px 0;
  letter-spacing: 2px;
  text-transform: uppercase;
  color:black;
  font-family: "Poppins", sans-serif;
}
.section-title h2::after {
  content: "";
  width: 120px;
  height: 1px;
  display: inline-block;
  background: black;
  margin: 4px 10px;
}
.section-title p {
  margin: 0;
  margin: 0;
  font-size: 36px;
  font-weight: 700;
  font-family: "Playfair Display", serif;
  color:lightseagreen;
}

 </style>
 

