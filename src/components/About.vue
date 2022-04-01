<template >
   <section id="about" class="about">
      <div class="container" data-aos="fade-up">
    <div class="section-title">
          <h2>ABOUT</h2>
          <p>ABOUT ME</p>
        </div>
    
        <div class="row">
          <div class="col-lg-6 order-1 order-lg-2" data-aos="zoom-in" data-aos-delay="100">
            <div class="about-img">
               <img src="" alt="">
            </div>
          </div>
          <div class="col-lg-6 pt-4 pt-lg-0 order-2 order-lg-1 content">
            <h3>Web Developer</h3>
            <p>
              I am an insipring web developer. My passion for computer & coding was introduced when I was attending a career exhibition that's when I  became super immersed with Technology development in this particular industry.
            </p>
           <div class="row">
              <div class="col-lg-6">
                <ul class="list">
                  <li><i class="bi bi-chevron-right"></i> <strong>Birthday:</strong> <br><span>29 July 2000</span></li><br>
                  <li><i class="bi bi-chevron-right"></i> <strong>languages:</strong> <br><span>IsiXhosa & English</span></li><br>
                  <li><i class="bi bi-chevron-right"></i> <strong>Phone:</strong> <br><span>+27780048135</span></li><br>
                </ul>
              </div>
              <div class="col-lg-6">
                <ul class="list">
                   <li><i class="bi bi-chevron-right"></i> <strong>Email:</strong><br> <span>uqolweni@gmail.com</span></li><br>
                  <li><i class="bi bi-chevron-right"></i> <strong>Freelance:</strong><br> <span>Available</span></li><br>
                  <li><i class="bi bi-chevron-right"></i> <strong>City:</strong><br> <span> Western Cape,Cape Town</span></li><br>

                </ul>
              </div>
           </div>
          
           <p>
           Currently I'm a student that aspires to be a great full-stack developer. My greatest aspiration is not only to learn, but to open door for other female coders such as me in this male dominated industry. I am eager to learn, always keen on inventing my self into becoming the best within my capabilities. Social active individual that takes initiative in always improvising where needed.</p>
          </div>
        </div>

      </div>
    </section><!-- End About Section -->


</template>
<script>
export default {
    
}
</script>
<style scoped>
*{
  color:black;
}
li span{
  color:black;
  font-weight: bold

}

   .about {
  /* background: url(https://images.pexels.com/photos/57690/pexels-photo-57690.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1) center center; */
  background-size: cover;
  position: relative;
  padding: 80px 0;
 
}
.about:before {
  content: "";
  /* background: rgba(0, 0, 0, 0.8); */
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
}
.about .about-img {
  position: relative;
  transition: 0.5s;
}
.about .about-img img {
  max-width: 100%;
  border: 4px solid rgba(255, 255, 255, 0.2);
  position: relative;
}
.about .about-img::before {
  position: absolute;
  left: 20px;
  top: 20px;
  width: 60px;
  height: 60px;
  z-index: 1;
  content: "";
  border-left: 5px solid lightseagreen;
  border-top: 5px solid lightseagreen;
  transition: 0.5s;
}
.about .about-img::after {
  position: absolute;
  right: 20px;
  bottom: 20px;
  width: 60px;
  height: 60px;
  z-index: 2;
  content: "";
  border-right: 5px solid lightseagreen;
  border-bottom: 5px solid lightseagreen;
  transition: 0.5s;
}
.about .about-img:hover {
  transform: scale(1.03);
}
.about .about-img:hover::before {
  left: 10px;
  top: 10px;
}
.about .about-img:hover::after {
  right: 10px;
  bottom: 10px;
}
.about .content h3 {
  font-weight: 600;
  font-size: 26px;
}
.about .content ul {
  list-style: none;
  padding: 0;
}
.about .content ul li {
  padding-bottom: 10px;
}
.about .content ul i {
  font-size: 20px;
  padding-right: 4px;
  color: #cda45e;
}
.about .content p:last-child {
  margin-bottom: 0;
}
@media (min-width: 1024px) {
  .about {
    background-attachment: fixed;
  }
}

 
</style>