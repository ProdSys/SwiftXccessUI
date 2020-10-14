<template>
    <div class="paymentanalysis">
            <div class="payment_container">
                <div class="paymentanalysis__header">
                <h5> Payment analysis</h5>
            </div>
            <div class="paymentanalysis__mid">
                <listvalue/>
                <listvalue/>
                <listvalue/>
                <listvalue/>
                
            </div>
            <div class="paymentanalysis__footer">
                <div class="paymentanalysis__footer_values">
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


.paymentanalysis {
    display: flex;
    justify-content: center;
    align-content: center;
    padding: 9px;
    width: 100%;
    flex-direction: column;
    background-color: #dfe7fd;

}

.paymentanalysis__header {
    display: flex;
    height: 5vh;
    width: 100%;
    background-color: #edf6f9;
    align-items: center;
    
    
}
.paymentanalysis__header > h5 {

    margin-left:5px;
    font-weight: bold;
    font-size: medium;


}
.paymentanalysis__mid{
    height: 25vh;
    width: 100%;
    background-color: whitesmoke;
    overflow: hidden;
}
.paymentanalysis__footer {
    height: 5vh;
    width: 100%;
    background-color:#edf6f9;

}

.paymentanalysis__footer_values {
    display: flex;
    height: 100%;
    justify-content: center;
    justify-content: start;

    align-items: center;
}
.paymentanalysis__footer_values > p {
    padding: 5px;
    margin-left:0;
    font-weight: lighter;;
    font-size: small;
    letter-spacing: 1px;
}
.payment_container {
    box-shadow: 0 0 5px 0 #888888;
}
</style>
