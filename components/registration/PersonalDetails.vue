<template>
 <div class="registration__container ">
   <div class="registration__left">
     <div class="registration__welcome">
       <h3>Welcome to</h3>
       <h5>TSB Business Banking</h5>
       <h6>Application tracker</h6>
     </div>

     <div class="registration__timeline__container">
       <ul class="registration__timeline">
         <li>Search for your company</li>
         <li>Your Personal Details</li>
         <li>Your Business / organization Details</li>
         <li>Your banking Services</li>
         <li>Your Application Summary</li>
         <li>Your Signatory mandate</li>
         <li>Your terms and conditions</li>
         <li>Next Steps</li>
       </ul>
     </div>
   </div>
   <div class="registration__right"></div>
 </div>
</template>

<script>
import { Timeline, TimelineItem, TimelineTitle } from "vue-cute-timeline";

export default {
  components: {
   
  }
};
</script>


<style scoped>


.registration__container{
  height: 80vh;
  display: flex;
  background-color:whitesmoke;
  
  margin: 5vh;
}

.registration__left{
  flex:0.36;
  display: flex;
  flex-direction: column;
  background-color:#f0efeb;
  
}


.registration__welcome {
  display: flex;
  color: #023e8a;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 30%;
}


.registration__timeline__container {
  display: flex;
  margin-top: 10px;
  background-color:f0efeb;
  height: 50%;
  position: relative;
  align-items: center;
  justify-content: center;

}


.registration__timeline{
  
  position: absolute;
  
}
.registration__timeline > ul {
   list-style-type: none;
    position: relative;
}

.registration__timeline:before {
    content: ' ';
    background: #d4d9df;
    display: inline-block;
    position: absolute;
    left: 29px;
    width: 2px;
    height: 100%;
    z-index: 400;
}

.registration__timeline > li {
    margin: 20px 0;
    padding-left: 20px;
}

.registration__timeline > li:before {
  
   content: ' ';
    background: white;
    display: inline-block;
    position: absolute;
    border-radius: 50%;
    border: 3px solid #22c0e8;
    left: 20px;
    width: 20px;
    height: 20px;
    z-index: 400;
}



</style>
