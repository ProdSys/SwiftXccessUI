<template>
    <div class="dashboard">
        <div class="dashboard__header">
            <div class="log_date_icon">
                <div class="dashboard__logo">
                    <img src="/img/logo.svg" alt="">
                </div>
                
                <div class="dashboard__date_container">
                    <h4>09:10</h4>
                <div class="dashboard__date">
                    <p>Satuarday</p>
                    <p>05 September 2020</p>
                </div>
                </div>

                <div class="dashboard__icons__top">
                    <img src="/img/notification.svg" alt="">
                    <img src="/img/search.svg" alt="">
                    <img src="/img/message.svg" alt="">
                    <img src="/img/close.svg" alt="">
                </div>

            </div>
            <div class="avator_card_button">

                <div class="avatar_container">
                    <div class="dashboard__avator">
                    <img src="/img/myAvatar.svg" alt="">
                </div>
                <div class="avatar__name">
                    <h3>Jone Doe</h3>
                </div>

                </div>

                <div class="dashboard__card__container">

                <div class="dashboard__card">
                    <cards/>
                    <cards/>
                    <menu/>
                </div>

                <div class="dashboard__button">

                    <h4>Cards</h4>
                    <img src="/img/plusbutton.svg" alt="">
                    <img src="/img/removebutton.svg" alt="">

                </div>

                </div>
                
            </div>
        </div>
        <div class="dashboard__content">

            <div class="dashboard__content__menu">
                <menus/>
            </div>

            <div class="dashboard__content__midtable">
                <div class="dashboard__content__navigation">
                    <p>Dashboard > Accounts > Recent transactions </p>
                </div>
                <div class="dashboard__content__resenttransactions">
                    <div class="dashobard__table">
                        <resenttransaction/>
                    </div>
                </div>
            </div>

            <div class="dashboard__content__rigttable">
                <paymentanalysis/>
            </div>
        </div>    
    </div>    
</template>

<script>

import cards from '~/components/cards/card';
import menus from '~/components/menus/menu';
import resenttransaction from '~/components/table/resenttransactions';
import paymentanalysis from '~/components/table/paymentanalysis';


export default {
  components: {
   cards,
   menus,
   resenttransaction,
   paymentanalysis,
  
}
};
</script>


<style scoped>

.dashboard {
    display: flex;
    height: 90vh;

    background-color:#caf0f8;
    margin: 2%;
    flex-direction: column;

}

.dashboard__header {
  
background-color: #023e8a;
flex: 0.3;
padding-top: 10px;
}

.log_date_icon {
    color: white;
    display: flex;
    width: 100%;
    background-color: #023e8a;
    justify-content: space-between;
    padding-left: 20px;
    padding-right: 20px;

}

.dashboard__icons__top {

   align-self: center;
   display: flex;
   width: 15%;
   justify-content: space-evenly;
   }

dashboard__icons__top > img {
    justify-content: space-between;
}


.dashboard__date {
    margin-top: 10px;
}
.dashboard__date > p {

    margin: 0 auto;
    font-size: 13px;
    font-weight: 100;
} 

.dashboard__date_container{
    display: flex;
    width: 20%;
}

.dashboard__date_container > h4{
   margin-top: 15px;
   margin-right: 5px;
}


.dashboard__logo > img{

    width: 200px;
    margin-top:5px;

}

.avator_card_button {
    display: flex;
    background-color: #023e8a;
    height: 100%;
    justify-content:space-around ;
    
    
    
}


.dashboard__avator > img {
    max-width: 100%;
    max-height: 100%;
  

}

.dashboard__avator{
    
    margin-left: 5%;
    border-radius:50% ;
    width: 100px;
    height: 100px;
    background-color: #023e8a;
    object-fit: cover;
    overflow: hidden;
    align-self: center;
    margin-bottom:1vh ;
 

}


.dashboard__card__container {
    display: flex;
    margin-right: 30px;
}
.dashboard__card{
    margin: 0;
    display: flex;
    background-color: #023e8a;
    width: 100vh;
    overflow: hidden;
    justify-content: center;
    align-items: center;

    
}

.dashboard__button{

    display: flex;
    background-color: #023e8a;
    width: 10vh;
    height: 100%;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color:white;
    
}

.dashboard__button * {
    margin-bottom: 15px;
}

.dashboard__button > img {
    max-width:200px;
    max-height: 200px;
}


.avatar_container {
    display: flex;
    flex-direction: column;
    justify-content: center;
}
.avatar__name > h3 {
    color: white;
}

.dashboard__content{

    display: flex;
    background-color: #dfe7fd;
    margin-top: 3%;
    width: 100%;
    height: 100%;

}

.dashboard__content__menu{
    flex: 0.25;
    background-color: #dfe7fd;
    height: 100%;
    

}

.dashboard__content__midtable {
    display: flex;
    flex-direction: column;
    flex:0.45;
    background-color: #dfe7fd;
    display: flex;
    height: 100%;

}

.dashboard__content__rigttable {
    display: flex;
    flex:0.30;
    background-color:purple;
    height: 100%;
    justify-content: center;
    align-content: center;


}



.dashboard__content__navigation {
    display: flex;
    margin-top: 10px;

    flex:0.07;
    height: 20px;
    background-color: #dfe7fd;
    align-items: center;
    width: 100%;

}

.dashboard__content__navigation > p {
    margin-top: 10px;
}

.dashboard__content__resenttransactions {
margin-top: 20px;
flex: 0.8;
}


.dashboard__button > img {
    width: 30px;
}

.dashboard__button > h4 {
    font-weight: 100;
    font-size: medium;
}
</style>
