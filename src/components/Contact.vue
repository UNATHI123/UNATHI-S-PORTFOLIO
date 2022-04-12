<template>

    <section id="contact" class="contact">
      <div class="container" data-aos="fade-up">

        <div class="section-title">
          <h2>Contact</h2>
          <p>CONTACT ME</p>
        </div>
      </div>

      <div class="container" data-aos="fade-up">

        <div class="row mt-5">

          <div class="col-lg-4">
            <div class="info">
              <div class="address">
                <i class="bi bi-geo-alt"></i>
                <h4>Location:</h4>
                <p>Western Cape, Cape Town</p>
              </div>

      

              <div class="email">
                <i class="bi bi-envelope"></i>
                <h4>Email:</h4>
                <p>unathiqolweni77@gmail.com</p>
              </div>

              <div class="phone">
                <i class="bi bi-phone"></i>
                <h4>Call:</h4>
                <p>+27 780 048 135</p>
              </div>

            </div>

          </div>

          <div class="col-lg-8 mt-5 mt-lg-0">

            <form   @submit.prevent="handleSubmit" class="php-email-form">
              <div class="row">
                <div class="col-md-6 form-group">
                  <input type="text" name="name" class="form-control" id="name" placeholder="Your Name" required v-model="text">
                </div>
                <div class="col-md-6 form-group mt-3 mt-md-0">
                  <input type="email" class="form-control" name="email" id="email" placeholder="Your Email" required v-model="email">
                </div>
              </div>
              <div class="form-group mt-3">
                <input type="text" class="form-control" name="subject" id="subject" placeholder="telephone" required v-model="tel">
              </div>
              <div class="form-group mt-3">
                <textarea class="form-control" name="message" rows="8" placeholder="Message" required v-model="textarea"></textarea>
              </div>
              <div class="my-3">
                <div class="loading">Loading</div>
                <div class="error-message"></div>
                <div class="sent-message">Your message has been sent. Thank you!</div>
              </div>
              <div class="text-center">
                <button type="submit">Send Message</button></div>
            </form>

          </div>

        </div>

      </div>
    </section>

</template>
<script>

export default {
 data(){
	 return{
		 text:"",
		 email:"",
		 tel:"",
		 textarea:""
		
	 }
 } ,
 methods:{
	handleSubmit(){
   console.log(this.text,this.email,this.tel,this.textarea),
    fetch('https://unathi-api.herokuapp.com/contact', {
  method: 'POST',
  body: JSON.stringify({
   text:  this.text,
   email: this.email,
   tel: this.tel,
   textarea: this.textarea
   }),
  headers: {
    'Content-type': 'application/json; charset=UTF-8',
  },
})
  .then((response) => response.json())
  .then((json) => alert(json.msg))
  .catch((e)=>alert(e.msg));
		
	 },
 }  
}
</script>
<style scoped >
    .contact .info {
  width: 100%;
}
.contact .info i {
  font-size: 20px;
  float: left;
  width: 44px;
  height: 44px;
  background: lightseagreen;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50px;
  transition: all 0.3s ease-in-out;
}
.contact .info h4 {
  padding: 0 0 0 60px;
  font-size: 18px;
  font-weight: 500;
  margin-bottom: 5px;
  font-family: "Poppins", sans-serif;
}
.contact .info p {
  padding: 0 0 0 60px;
  margin-bottom: 0;
  font-size: 14px;
  color: #000;
}
.contact .info .open-hours, .contact .info .email, .contact .info .phone {
  margin-top: 40px;
}
.contact .php-email-form {
  width: 100%;
}
.contact .php-email-form .form-group {
  padding-bottom: 8px;
}
.contact .php-email-form .validate {
  display: none;
  color:lightseagreen;
  margin: 0 0 15px 0;
  font-weight: 400;
  font-size: 13px;
}
.contact .php-email-form .error-message {
  display: none;
  color: #fff;
  background: lightseagreen;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}
.contact .php-email-form .sent-message {
  display: none;
  color: #fff;
  background: #18d26e;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}
.contact .php-email-form .loading {
  display: none;
  text-align: center;
  padding: 15px;
}
.contact .php-email-form .loading:before {
  content: "";
  display: inline-block;
  border-radius: 50%;
  width: 24px;
  height: 24px;
  margin: 0 10px -6px 0;
  border: 3px solid ;
  border-top-color: #1a1814;
  -webkit-animation: animate-loading 1s linear infinite;
  animation: animate-loading 1s linear infinite;
}
.contact .php-email-form input, .contact .php-email-form textarea {
  border-radius: 0;
  box-shadow: none;
  font-size: 14px;
  background: beige;
  border-color: #000;
  color:black;
}
.contact .php-email-form input::-moz-placeholder, .contact .php-email-form textarea::-moz-placeholder {
  color: #a49b89;
}
.contact .php-email-form input::placeholder, .contact .php-email-form textarea::placeholder {
  color: #a49b89;
}
.contact .php-email-form input:focus, .contact .php-email-form textarea:focus {
  border-color: lightseagreen;
}
.contact .php-email-form input {
  height: 44px;
}
.contact .php-email-form textarea {
  padding: 10px 12px;
}
.contact .php-email-form button[type=submit] {
  background: lightseagreen;
  border: 0;
  padding: 10px 35px;
  color: #fff;
  transition: 0.4s;
  border-radius: 50px;
}
.contact .php-email-form button[type=submit]:hover {
  background: lightseagreen;
}
@-webkit-keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
@keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
</style>