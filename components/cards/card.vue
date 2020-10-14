<template>
 <div class="cards">
 
     
     <div class="card__leftside">
         <div class="card_leftside_content">
             <div class="card_leftside_content_balance_icon">
                 <img src="/img/balance.svg" alt="">
                <img src="/img/currancy.svg" alt="">
             </div>
         </div>
     </div>

     <div class="card__rightside">
         <div class="card__rightside__top">
             <div class="card_rightside_top_cab">
                 <h4>Current Account</h4>
                 <img src="/img/dotButton.svg" alt="">
             </div>

            <div class="card_rightside_top_ammount">
                <h3> $145673</h3>
            </div>

            <div class="card_rightside_top_income_expense">
                <p>Income</p>
                <p>Expense</p>
            </div>

            <div class="card_rightside_top_inc_exp_numbers">
                <div class="income">
                    <img src="/img/income.svg" alt="">
                    <p>$123456</p>
                </div>

                <div class="income">
                    <img src="/img/expense.svg" alt="">
                    <p>$323456</p>
                </div>
            </div>

         </div>
         <div class="card__rightside__bottom">
             <div class="card__rightside__bottom_view_cards">
                 <div class="bottom_view_card_holder">
                     <img src="/img/viewcard.svg" alt="">
                     <p>View Cards</p>
                 </div>

                 <div class="bottom_view_card_holder">
                     <img src="/img/link.svg" alt="">
                     <img src="/img/point.svg" alt="">
                 </div>
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


h4 {
    font-weight:100;
    font-size: medium;
}

h3 {
    font-weight:bold;
    font-size: medium;
}



.cards {
    margin: 1px;
    display: flex;
    width: 280px;
    height: 200px;
    background-color: aliceblue;
    border-radius: 20px;
    margin-left:10px;
    margin-right: 10px;
}
.card__leftside {
    flex: 0.1;
    background-color: #03045e;
    height: 100%;
    border-radius: 20px 0 0 20px ;
    color: white;
}

.card__rightside {
    flex:0.9;
    background-color: #ade8f4;
    border-radius: 0 20px 20px 0 ;
    
}

.card_leftside_content {
    display: flex;
    height: 100%;
    flex-direction: column;
    justify-content: space-between;
    align-content: center;
}

h3 {
    margin: 0;
}

.card_leftside_content_balance_icon {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    height: 100%;
    
}


.card_leftside_content_balance_icon > h3 {
    margin-bottom: 0;
    letter-spacing: 1px;
    transform: rotate(-90deg);

  
}
.card_leftside_content_balance_icon > img {
    margin: 10px;
    width: 30px;
    align-self: center;
    margin-bottom: 10px;
    

}


.card__rightside {
    display: flex;
    background-color:#ade8f4 ;
    flex-direction: column;
    overflow: hidden;

}

.card__rightside__top {
    flex:0.7;
    background-color:#ade8f4;
    
}
.card_rightside_top_cab {
    margin: 15px;
    display: flex;
    justify-content: space-around;
}
.card_rightside_top_ammount {
    display: flex;
    justify-content: center;
}

.card_rightside_top_income_expense{
    margin: 0;
    display: flex;
    justify-content: space-around;
    background-color: #ade8f4;
}

.card_rightside_top_inc_exp_numbers {
    background-color:#ade8f4;
    margin: 0;
    display: flex;
    justify-content: space-around;
}

.income {
    
    display: flex;
    align-content: center;

}

.income > img {
    background-color:#ade8f4;
    width: 20px;
    height: 20px;
    margin-top: 2px;
    border-radius: 50%;    

}

.income > p {
    margin-left: 5px;
}

.card__rightside__bottom {
    display: flex;
    flex:1;
}

.card__rightside__bottom_view_cards {
    display: flex;
    flex: 1;
    justify-content: space-between;
}

.bottom_view_card_holder {
    display: flex;
    margin: 2px;
    justify-content: space-between;
    
}

.bottom_view_card_holder > p {
    margin-top: 8px;
    margin-left: 5px;
}

.bottom_view_card_holder > img {
    margin-left: 10px;
    margin-bottom: 9px;
    margin-right:7px;
    width: 20px;
}


</style>
