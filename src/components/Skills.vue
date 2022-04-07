<template >
     <section id="skills" class="skills">
      <div class="container" data-aos="fade-up">

        <div class="section-title">
          <h2>Skills</h2>
          <p>SOFT SKILLS </p>
        </div>

        <div class="row">

          <div class="col-lg-4">
            <div class="box" data-aos="zoom-in" data-aos-delay="100">
              <span>01</span>
              <h4>TEAM WORK</h4>
              <p>
                <ul>
                  <li>Collaboration</li>
                   <li>Coordination</li>
                    <li>Idea exchange</li>
                     <li>Mediation</li>

                </ul>
              </p>
            </div>
          </div>

          <div class="col-lg-4 mt-4 mt-lg-0">
            <div class="box" data-aos="zoom-in" data-aos-delay="200">
              <span>02</span>
              <h4>COMMUNICATION</h4>
              <p> <ul>
                <li> Verbal communication</li>
                <li>Written communication</li>
                <li>Presentation</li>
                <li>Active listening</li>
                </ul>
                </p>

            </div>
          </div>

          <div class="col-lg-4 mt-4 mt-lg-0">
            <div class="box" data-aos="zoom-in" data-aos-delay="300">
              <span>03</span>
              <h4>TIME MANAGEMENT</h4>
              <p><ul>
                <li>Organization</li>
              <li>Prioritizing</li>
             <li>Planning </li>
             <li>Goal setting</li>
              </ul>
               </p>
            </div>
          </div>

        </div>
      </div>
       <!-- ======= Skills Section ======= -->
    <section id="skillz" class="skillz">
      <div class="container" data-aos="fade-up">

        <div class="section-title">

          <p>Technical Skills</p>
        </div>

        <div class="row skillz-content">

          <div class="col-lg-6">

            <div class="progress">
              <span class="skill">HTML <i class="val">Proficient</i></span>
              <div class="progress-bar-wrap">
                <div class="progress">
  <div class="progress-bar w-75" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
</div></div>
            </div>

            <div class="progress">
              <span class="skill">CSS <i class="val">Proficient</i></span>
              <div class="progress-bar-wrap">
              <div class="progress">
  <div class="progress-bar w-75" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
</div> </div>
            </div>

            <div class="progress">
              <span class="skill">JavaScript <i class="val">Intermdiate</i></span>
              <div class="progress-bar-wrap">
               <div class="progress">
  <div class="progress-bar w-50" role="progressbar" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100"></div>
</div></div>
            </div>
            <div class="progress">
              <span class="skill">mysql <i class="val">Proficient</i></span>
              <div class="progress-bar-wrap">
                <div class="progress">
  <div class="progress-bar w-75" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
</div> </div>
            </div>

          </div>

          <div class="col-lg-6">


            <div class="progress">
              <span class="skill">Vue.JS <i class="val">Intermdiate</i></span>
              <div class="progress-bar-wrap">
                <div class="progress">
  <div class="progress-bar w-50" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
</div></div>
            </div>

            <div class="progress">
              <span class="skill">GIT <i class="val">Intermdiate</i></span>
              <div class="progress-bar-wrap">
               <div class="progress">
  <div class="progress-bar w-75" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
</div> </div>
            </div>
    
            
            <div class="progress">
              <span class="skill">NODE <i class="val">Intermdiate</i></span>
              <div class="progress-bar-wrap">
               <div class="progress">
  <div class="progress-bar w-50" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
</div> </div>
            </div>
            <div class="progress">
              <span class="skill">MONGO DB <i class="val">Proficient</i></span>
              <div class="progress-bar-wrap">
               <div class="progress">
  <div class="progress-bar w-75" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
</div> </div>
            </div>

         

          </div>  
        </div>

      </div>
    </section><!-- End Skills Section -->



     </section>
     
</template>
<script>
export default {
    
}
</script>
<style scoped >
    .skills .box {
  padding: 50px 30px;
  box-shadow: 0px 2px 15px rgba(0, 0, 0, 0.1);
  transition: all ease-in-out 0.3s;
  /* background: #; */
}
.skills .box span {
  display: block;
  font-size: 28px;
  font-weight: 700;
  color:lightseagreen;
}
.skills .box h4 {
  font-size: 24px;
  font-weight: 600;
  padding: 0;
  margin: 20px 0;
  color:#000;
}
.skills .box p {
  color: #aaaaaa;
  font-size: 15px;
  margin: 0;
  padding: 0;
}
.skills .box:hover {
  background: lightgray;
  padding: 30px 30px 70px 30px;
  box-shadow: 10px 15px 30px rgba(0, 0, 0, 0.18);
}
.skills .box:hover span, .skills .box:hover h4, .skills .box:hover p {
  color:orangered;
}

.skillz .progress {
  height: 60px;
  display: block;
  background: none;
  border-radius: 0;
}
.skillz .progress .skill {
  padding: 10px 0;
  margin: 0 0 6px 0;
  text-transform: uppercase;
  display: block;
  font-weight: 600;
  font-family: "Poppins", sans-serif;
  color: #222222;
}
.skillz .progress .skill .val {
  float: right;
  font-style: normal;
}
.skillz .progress-bar-wrap {
  background: #f3f3f3;
}
.skillz .progress-bar {
  width: 1px;
  height: 10px;
  transition: 0.9s;
  background-color: #34b7a7;
}

</style>