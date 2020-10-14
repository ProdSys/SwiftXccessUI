<template>
  <div id="main_login_div" style="margin-top:10%;">
    <div id="login">
      <div id="center_div" class="row">

        <div id="center_div">
          <div class="col pass_user">
            <div class="col">
              <div class="row top_handler">
                <img src="/img/fastAndFree.svg" alt="" width="164px"
                  style="margin-bottom:20px;margin-left:41%; padding-top:50%;">

              </div>
              <div class="row ">
                <img src="/img/simleAndQuick.svg" alt="" width="150px" style="margin-bottom:20px;margin-left:40%; ">

              </div>
              <div class="row ">
                <img src="/img/termsOfUse.svg" alt="" width="150px" style="margin-bottom:20px;margin-left:40%; ">

              </div>
              <div class="row ">
                <img src="/img/privacyPolicy.svg" alt="" width="115px" style="margin-bottom:20px;margin-left:40%; ">

              </div>
            </div>
          </div>
        </div>

        <div id="loginCover" class="col"><img id="loginCoverImg" src="/img/loginCover.svg" style="width:700px" /></div>
        <div id="center_div">
          <div id="sideAbit" class="col pass_user">
            <div class="col">
              <div class="row top_handler">
                <h1 id="welcome">Welcome back !</h1>
              </div>
              <div class="row">
                <h5>Please login to your account</h5>
              </div>
              <div id="email_input" class="row"><input class="form-control form-control-lg " type="text"
                  placeholder="Email" height="50"></div>
              <div id="password_input" class="row"><input class="form-control form-control-lg" type="text"
                  placeholder="Password" height="50"></div>
              <div id="login_buttons_handler">
                <div class="row">
                  <div class="col-sm-8"><img id="sign_in_button" src="/img/siginButton.svg" alt=""></div>
                  <div class="col-sm-4"><img id="arrow_button" src="/img/arrow.svg" alt=""></div>
                </div>
                <div class="row">
                  <b-link to="/register" class="text-decoration-underline text-grey">
                    <div class="col-sm-12"><img id="open_An_Account" src="/img/openAccount.svg" alt=""></div>
                  </b-link>


                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {}
</script>
<style scoped>
  #center_div {
    margin-right: 5%;
  }


  @media only screen and (min-width: 1500px) {

    .top_handler {


      margin-top: 40%;
    }



  }



  @media only screen and (max-width: 1600px) {


    #sideAbit {
      margin-left: 30%;
    }



  }


  @media only screen and (max-width: 1400px) {

    #welcome {
      color: brown;
    }


    #loginCoverImg {
      display: none;
    }



  }






  @media only screen and (max-width: 3000px) {

    .top_handler {

      margin-top: 40%;

    }


  }

  #loginCover {
    height: 10em;
    position: relative;
    margin-left: 5%;
  }

  #loginCover img {
    margin: 0;

    position: absolute;
    top: 170%;
    left: 50%;
    margin-right: -50%;
    transform: translate(-50%, -50%)
  }

  #email_input {
    margin-top: 20px;

  }

  #password_input {
    margin-top: 20px;
  }

  #arrow_button {
    width: 70%;
  }


  #arrow_button:hover {
    width: 71%;
  }


  #sign_in_button {
    width: 90%;

  }

  #sign_in_button:hover {
    width: 91%;
  }

  #open_An_Account {
    width: 80%;
  }

  #open_An_Account:hover {
    width: 81%;
  }

  #Email {
    width: 50%;
  }

  #login_buttons_handler {

    margin-top: 5%;

  }


  #login_div {
    margin: 3px;
    width: 100%;
    margin-top: 20%;

  }



  #main_login_div {
    padding: 2%;



  }

  .pass_user {

    margin: 1%;
  }

  #login {

    background-color: whitesmoke;
    padding: 1%;
    box-shadow: rgba(2, 2, 2, 0.1) 0 0 10px;
    border-radius: 50px 20px;
    ;

  }

  body {
    background-color: rgb(163, 182, 218);
  }
</style>