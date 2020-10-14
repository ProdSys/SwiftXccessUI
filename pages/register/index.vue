<template>
  <div id="maindivregis" class="container">

    <div><img src="/img/logo.svg" alt="" style="margin-bottom:10px;"></div>
    <div><p id="test">Will you be using OnVirtual Cards for personal or business use?</p>
    </div>

    <div id="cardsrow " class="row">
      <div class="col">
        <div class="card cardShadow" style="width: 20rem;">
          <div class="card-body">
            <h5 class="card-title whiteText">Business</h5>
            <p class="card-text whiteText">Issue cards and assign them to employees. You decide when to stop cards or add more funds</p>
            <b-link to="/register/corporate" class="whiteText">Cotinue</b-link>

          </div>
        </div>
      </div>
      <div class="col">
        <div class="card cardShadow" style="width: 20rem;" >
          <div class="card-body">
            <h5 class="card-title whiteText">Personal</h5>
            <p class="card-text whiteText">Take control of your online purchases and shop securely without exposing your bank card</p>
            <b-link to="/register/consumer" class="whiteText">Cotinue</b-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<style >

  body{
  background-color:rgb(163, 182, 218);
}

 
  #cardsrow{
    margin-left: 20px;
    width: 100%;
    background-color: whitesmoke;
  }




 @media only screen and (max-width: 3000px) {

#test{
  color: brown;
}

      #maindivregis {
    text-align: center;
    position: absolute;
    width: 50%;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    padding: 10px;
      

  }



  }


  .cardShadow{
   

      background-color:rgb(34, 34, 153);
    padding: 2%;
    box-shadow: rgba(27, 17, 17, 0.4) 0 0 10px;
  border-radius: 50px 20px;
  }
   .whiteText {
     color: white;
   }
</style>