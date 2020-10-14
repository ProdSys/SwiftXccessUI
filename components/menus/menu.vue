<template>
 <div class="menus">
 
     <div class="menus__all__information">
         <h4>Accounts</h4>
         <div class="menus__all__accounts">
             <div class="menus__all__accounts__container">
                 <img src="/img/allacounticon.svg" alt="">
                 <span>All Acounts</span>

             </div>
         </div>

        <div class="menus__transactions">
             <div class="menus__transactions__container">
                 <img src="/img/transactions.svg" alt="">
                 <span>Transactions</span>
             </div>
         </div>


          <div class="menus__cards">
             <div class="menus__cards__container">
                 <img src="/img/cardsicon.svg" alt="">
                 <span>Cards</span>
             </div>
         </div>

        <h4>Transactions</h4>

        <div class="menus__paybill">
             <div class="menus__paybill__container">
                 <img src="/img/paybill.svg" alt="">
                 <span>Pay Bill</span>
             </div>
         </div>

         <div class="menus__atmwithdrawal">
             <div class="menus__atmwithdrawal__container">
                 <img src="/img/atmwithdrawal.svg" alt="">
                 <span>ATM withdrawal</span>
             </div>
         </div>

         <div class="menus__requestmony">
             <div class="menus__requestmony__container">
                 <img src="/img/requestmoney.svg" alt="">
                 <span>Request Money</span>
             </div>
         </div>

         <h4>Transfers</h4>
         
         <div class="menus__betweencard">
             <div class="menus__betweencard__container">
                 <img src="/img/betweencards.svg" alt="">
                 <span>Between Card</span>
             </div>
         </div>

         <div class="menus__bankaccount">
             <div class="menus__bankaccount__container">
                 <img src="/img/bankaccount.svg" alt="">
                 <span>Bank account</span>
             </div>
         </div>

         <div class="menus__mobilenumber">
             <div class="menus__mobilenumber__container">
                 <img src="/img/mobilenumber.svg" alt="">
                 <span>Mobile number</span>
             </div>
         </div>

         <div class="menus__messages">
             <div class="menus__messages__container">
                 <img src="/img/messagesicon.svg" alt="">
                 <span>Messages</span>
             </div>
         </div>

         <div class="menus__settings">
             <div class="menus__settings__container">
                 <img src="/img/settingsicon.svg" alt="">
                 <span>Settings</span>
             </div>
         </div>

         <div class="menus__logout">
             <div class="menus__logout__container">
                 <img src="/img/logouticon.svg" alt="">
                 <span>Logout</span>
             </div>
         </div>
         

     </div>
 </div>
</template>

<script>

export default {
 
};
</script>


<style scoped>



.menus {
   display: flex;
   flex-direction: column;
   align-items: center;
   height: 100%;
   width: 100%;
   background-color: #dfe7fd;
   
}

.menus__all__information {
    display: flex;
    flex-direction: column;
    justify-items: center;
    background-color: #cddafd;
    height: 100%;
    width: 80%;
    padding: 20px;
    justify-content: space-between;
    margin: 10px;
    box-shadow: 0 0 5px 0 #888888;
}

.menus__all__information > div > div:hover {
    background-color: #fff1e6;
    padding: 20px;
}

.menus__all__information > div > div > span {
    margin: 0;
    font-size: xx-small;
    font-weight: normal;
    letter-spacing: 1px;
    margin-bottom: 5px;
}

.menus__all__information > div > div > img {
   margin: 0;
   width: 14px;
}


h4 {
    margin: 0;
    padding: 0;
    font-weight: bold;
    font-size: medium;
    letter-spacing: 1px;
    margin-bottom: 2px;

}

</style>
