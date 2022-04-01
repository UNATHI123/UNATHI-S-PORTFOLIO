<template >
     <section id="skills" class="skills">
      <div class="container" data-aos="fade-up">

        <div class="section-title">
          <h2>Skills</h2>
          <p>HTML, CSS  & JAVASCRIPT </p>
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


</style>