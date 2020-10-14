<template>
    <div class="resentrans">
            <div class="resentrains_container">
                <div class="resentrans__header">
                <h5> Recent Account Transactions</h5>
            </div>
            <div class="resentrans__mid">
                <listvalue/>
                <listvalue/>
                <listvalue/>
                <listvalue/>
                
            </div>
            <div class="resentrans__footer">
                <div class="resentrans__footer_values">
                    <p>All</p>
                    <p>Paid</p>
                    <p>Pending</p>
                    <p>Cancelled</p>
                </div>
            </div>
            </div>
    </div>    
</template>

<script>

    import listvalue from '~/components/table/list';


export default {

  components: {
  listvalue,
  
}
};
</script>


<style scoped>


.resentrans {
    padding: 10px;
    display: flex;
    width: 100%;

    flex-direction: column;
    background-color:#dfe7fd ;
}

.resentrans__header {
    display: flex;
    height: 5vh;
    width: 100%;
    background-color: #edf6f9;
    align-items: center;
    
    
}
.resentrans__header > h5 {

    margin-left:5px;
    font-weight: bold;
    font-size: medium;


}
.resentrans__mid{
    height: 30vh;
    width: 100%;
    background-color:whitesmoke;
    overflow: hidden;
}
.resentrans__footer {
    height: 5vh;
    width: 100%;
    background-color:#edf6f9;

}

.resentrans__footer_values {
    display: flex;
    height: 100%;
    justify-content: center;
    justify-content: start;

    align-items: center;
}
.resentrans__footer_values > p {
    padding: 5px;
    margin-left:0;
    font-weight: lighter;;
    font-size: small;
    letter-spacing: 1px;
}

.resentrains_container{
    box-shadow: 0 0 5px 0 #888888;

}
</style>
