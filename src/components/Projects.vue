<template >
 <section id="projects" class="projects">
     <div class="container" data-aos="fade-up">

     <div class="section-title">
          <h2>Projects</h2>
          <P>MY WORK </P> 
       </div>
       <div class="row">
          <div class="col-lg-4 col-md-6" v-for="project of projects" :key="project>id">
            <div class="member" data-aos="zoom-in" data-aos-delay="100">
              <img :src= project.img class="img-fluid" alt="">
              <div class="member-info">
                <div class="member-info-content">
                  <h1>{{project.title}}</h1>
                  <span>{{project.details}}</span>
                  <h3>Click the icon</h3>
                </div>
                <div class="social">
                  <a  :href="project.live" target="_blank"><i class="bi bi-play-circle"></i></a>
                  <a :href="project.github" target="_blank"><i class="fa-brands fa-github"></i></a>
                  
                </div>
              </div>
            </div>
          </div>
     </div>
     </div>
 </section>
</template>
<script>
export default {
    data() {
        return {
            projects:[]
        }
    },
    mounted(){
        fetch('https://unathi-api.herokuapp.com/projects')
        .then(res => res.json())
        .then(data => {
          this.projects = data
          console.log(data)
          
          })
        .catch(err => console.log(err.message))
        
    }
}
</script>
<style scoped>
.img-fluid{
    height: 300px;
    width: 400px;
}

.projects .member {
  text-align: center;
  margin-bottom: 20px;
  background: #343a40;
  position: relative;
  overflow: hidden;
}
.projects .member .member-info {
  opacity: 0;
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
  transition: 0.2s;
}
.projects .member .member-info-content {
  position: absolute;
  left: 0;
  right: 0;
  bottom: 10px;
  transition: bottom 0.4s;
}
.projects .member .member-info-content h1 {
  font-weight: 700;
  margin-bottom: 2px;
  font-size: 18px;
  color: #fff;
}
.projects .member .member-info-content span {
  font-style: bold;
  display: block;
  font-size: 13px;
  color: #fff;
}
.projects .member .member-info-content h3 {
    color:#fff;
}
.projects .member .social {
  position: absolute;
  left: 0;
  bottom: -38px;
  right: 0;
  height: 48px;
  transition: bottom ease-in-out 0.4s;
  text-align: center;
  size: 10px;
}
.projects .member .social a {
  transition: color 0.3s;
  color: #fff;
  margin: 0 10px;
  display: inline-block;
}
.projects .member .social a:hover {
  color: #cda45e;
}
.projects .member .social i {
  font-size: 18px;
  margin: 0 2px;
}
.projects .member:hover .member-info {
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.9) 0%, rgba(0, 0, 0, 0.8) 20%, rgba(0, 212, 255, 0) 100%);
  opacity: 1;
  transition: 0.4s;
}
.projects .member:hover .member-info-content {
  bottom: 60px;
  transition: bottom 0.4s;
}
.projects .member:hover .social {
  bottom: 0;
  transition: bottom ease-in-out 0.4s;
}

</style>