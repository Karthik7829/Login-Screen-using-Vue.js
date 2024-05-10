
<template>
  <div class="bgimage">
    <div class="parentcontainer">
    <div class="container">
      <p class="logo1">MGM</p>
      <h4 class="logo2">Global</h4>
      <h4 class="logo3">Distribution</h4>
       <form @submit.prevent="submitForm">
      <h4 class="label1">Sign in</h4>
      <label class="label2">Email</label>
      <input type="email"  v-model="email" class="inpt1"  placeholder="Enter your email address"  required>
       <label class="label3">Password</label>
      <input class="inpt2" type="password" v-model="password" placeholder="Enter your password"  required>
      <img src="./assets/close-eye.png" class="closeeye"/>
      <h4 class="fgpswd" @click="forgotPassword">Forgot Password?</h4>
      <input type="checkbox" class="ckbx"/>
      <h4 class="label4">Keep me signed in for 30 days</h4>
      <button class="btn">SIGN IN</button>
      </form>
      <p class="label5">Read our Terms of Service</p>
      <i class="fa-solid fa-arrow-up-right-from-square"></i>
      <div class="btmcont1">
        <div class="btmcont2">
          <p class="label6">OTHER WAYS TO WATCH</p>
          <img src="./assets/apple-tv.png" class="appletv"/>
           <img src="./assets/ios-logo.png" class="ios"/>
            <img src="./assets/roku.png" class="roku"/>
            <img src="./assets/AmazonFire.png" class="AmazonFire"/>
            <p class="label7">Search for AppleTV+ FYC on your App Store</p>
        </div>
      </div>
    </div>
    </div>
  </div>
  
</template>





<style>
*{
  margin: 0;
  padding: 0;
  
}

body{
  width: 100%;
  height: 100%;
}
.bgimage{
  background-image: url("assets/banner.jpg");
  width: 100%;
  height: 100vh;
  background-size: cover;
  position: relative;
}

.bgimage::before{
  content: "";
  position: absolute;
  top: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.7);
}

.parentcontainer{
  display: flex;
  justify-content: center;
  align-items: center;
}

.container{
    width: 300px;
    height: 500px;
    gap: 0px;
    border-radius: 3px 3px 3px 3px;
    border: 3px 0px 0px 0px;
    opacity: 0.85px;
    background-color: white;
    margin: 30px;
    background: var(--Elements-Glass-Black,rgba(10, 10, 10, 1));
    border: 3px solid var(--Elements-Tamara-Black,rgba(24, 24, 24, 1));
    box-shadow: 10px 10px 15px 10pxrgba(0, 0, 0, 0.25);
}



.logo1{
  position: relative;
  font-size: 45px;
  font-weight: 400;
  text-align: center;
  left: -30px;
  top: 20px;
  font-family: "Kurale", serif;
  color: #FFFFFF;
}

.logo2{
  position: relative;
  left: 175px;
  top: -32px;
  font-size: 15.5px;
  font-weight: 600;
  font-family:  "Noto Sans", sans-serif;
  color: #FFFFFF;
}

.logo3{
  position: relative;
  left: 175px;
  top: -36px;
  font-size: 15.5px;
  font-weight: 600;
  font-family:  "Noto Sans", sans-serif;
  color: #FFFFFF;
}

.label1{
  position: relative;
  left: 29px;
  top: -10px;
  font-size: 21px;
  font-weight:600;
  font-family:  "Noto Sans", sans-serif;
  color: #FFFFFF;
}

.label2{
  position: relative;
  top: 2px;
  left: 29px;
  font-family:  "Noto Sans", sans-serif;
  font-size: 15px;
  font-weight: 600;
  color: #1A68FF;
}

.inpt1{
  position: relative;
  top: 30px;
  left: -10px;
  height: 30px;
  width: 235px;
  background-color:#1C1C1E;
  border: none;
  color: white;
}

::placeholder{
  position: relative;
  left: 12px;
  font-family:  "Noto Sans", sans-serif;
  font-weight: 400;
  color: #BCBCBC;
  font-size: 12px;
}

.label3{
  position: relative;
  top: 42px;
  left: 29px;
  font-family:  "Noto Sans", sans-serif;
  font-weight: 600;
  font-size: 15px;
  color: #1A68FF;
}

.inpt2{
  position: relative;
  top: 42px;
  left: 30.5px;
  height: 30px;
  width: 235px;
  background-color:#1C1C1E;
  border: none;
  color: white;
}

.closeeye{
  position: relative;
  height: 23px;
  width: 23px;
  top: 50px;
  left: 2px;
  color:#8E8E93;
  cursor: pointer;
}

.fgpswd{
  position: relative;
  top: 48px;
  left: 174px;
  font-family: Noto Sans;
  font-size: 11px;
  font-weight: 400;
  cursor: pointer;
  color: #BCBCBC;
}

.ckbx{
  position: relative;
  top: 78px;
  width: 16px;
  height: 16px;
  left: 32px;
  border-radius: 3px 0px 0px 0px;
  border: 2px 0px 0px 0px;
  background-color: #1C1C1E;
  font-weight: 100;
}

input[type="checkbox"]{
background-color: #1C1C1E;
}

.label4{
  position: relative;
  top: 57px;
  left: 56px;
  font-family: Noto Sans;
  font-size: 11px;
  font-weight: 500;
  color: #BCBCBC;
}

.btn{
  position: relative;
  top: 110px;
  height: 30px;
  width: 235px;
  left: 33px;
  background: var(--Primary-Electric-Blue, rgba(0, 87, 255, 1));
  border: none;
  color: #FFFFFF;
  font-family: Noto Sans;
  font-weight: 400;
  letter-spacing: 3px;
  cursor: pointer;
}

.label5{
  position: relative;
  top: 140px;
  font-size: 12px;
  left: 33px;
  font-family: Noto Sans;
  font-weight: 500;
  color:  #BCBCBC;
;
}

.fa-arrow-up-right-from-square{
  position: relative;
  top: 121.5px;
  left: 188px;
  font-size: 7px;
  color: #FFFFFF;
}

.btmcont1{
  width: 300px;
  height: 110px;
  position: relative;
  top: 164px;
  right: 3px;
  border-radius: 0px 0px 3px 3px;
  opacity: 0px;
  background-color: #2D3137;
  border: 3px solid var(--Elements-Tamara-Black, #181818);
}

.btmcont2{
  width: 300px;
  height: 76px;
  background-color: #24272C;
  position: relative;
  top: 34px;
}

.label6{
  position: relative;
  font-size: 8px;
  font-family: Noto Sans;
  font-weight: 500;
  color: #D5D5D5;
  text-align: center;
  top: 13px;
}

.appletv{
  position: absolute;
  width: 48px;
  top: 35px;
  left: 30px;
  cursor: pointer;
}

.ios{
   width: 36px;
   position: absolute;
   top: 28px;
   left: 99px;
   cursor: pointer;
}

.roku{
   width: 45px;
   position: absolute;
   top: 37px;
   left: 157px;
   cursor: pointer;
}

.AmazonFire{
   width: 45px;
   position: absolute;
   top: 29px;
   left: 222px;
   cursor: pointer;
}

.label7{
  position: relative;
  font-size: 8px;
  font-family: Noto Sans;
  font-weight: 500;
  color: #D5D5D5;
  text-align: center;
  top: 48px;
}


/*  Tablet   */
 @media only screen and (max-width: 768px) { 
  .container {
    width: 300px; 
    margin: 5px; 
  }
}

@media only screen and (max-width: 820px) { 
  .container {
    width: 300px; 
    margin: 95px; 
  }
}

@media only screen and (max-width: 1024px) { 
  .container {
    width: 300px; 
    margin: 10px; 
  }
} 

@media only screen and (max-width: 912px) { 
  .container {
    width: 300px; 
    margin: 40px; 
  }
}

@media only screen and (min-width: 540px) { 
  .container {
    width: 300px; 
    margin: 20px; 
  }
}
/*  Tablet   */


/* Mobile */
@media only screen and (max-width: 375px) {
  .container {
    width: 300px; 
    margin: 22px; 
    position: relative;
    left: 2px;
  }
}

@media only screen and (min-width: 414px) {
  .container {
    width: 300px; 
    margin: 110px; 
    position: relative;
    right: 10px;
  }
}

@media only screen and (min-width: 390px) {
  .container {
    width: 300px; 
    margin: 90px; 
  }
}

@media only screen and (min-width: 430px) {
  .container {
    width: 300px; 
    margin: 90px; 
    position: relative;
    right: 15px;
  }
}

@media only screen and (min-width: 412px) {
  .container {
    width: 300px; 
    margin: 130px; 
  }
}

@media only screen and (min-width: 360px) {
  .container {
    width: 300px; 
    margin: 55px; 
    position: relative;
    left: 5px;
  }
}

@media only screen and (min-width: 412px) {
  .container {
    width: 300px; 
    margin: 155px; 
    position: relative;
    left: 5px;
  }
}
/* Mobile */


/* Laptop */
@media only screen and (min-width: 1280px) {
  .container {
    width: 300px; 
    margin: 35px; 
  }
}



</style>

<script>
export default {
  data() {
    return {
      Email: 'karthik@gmail.com',
      Password: 'Karthik@7829',
      validEmail: true,
      validPassword: true
    };
  },
 methods: {
    submitForm() {
      this.validEmail = this.validateEmail();
      this.validPassword = this.validatePassword();
      if (this.validEmail && this.validPassword) {
        alert('Sucessfully Logged in:', this.email, this.password);
        window.location.assign("")
      }
      // // else{
      //   alert('Invalid Credentials:', this.email, this.password);
    },
    validateEmail() {
      return /\S+@\S+\.\S+/.test(this.email);
    },
    validatePassword() {
      return !!this.password;
    },
     forgotPassword() {
      alert("Recover Your Old Password Here..!");
    }
  }
};


</script>