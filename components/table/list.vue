<template>
    <div class="list">


        <div class="list_holder">

            <div class="list__start">
                <img src="/img/listvalue.svg" alt="img">
                <div class="list__values">
                    <h4>Cost Cafe</h4>
                    <p>Restaurant</p>
                </div>
            </div>

            <div class="list__midfirst">
                <div class="list__midfirst__vlaues">
                    <p>$2.40</p>
                    <p>Amount</p>
                </div>
            </div>

            <div class="list__midfirst">
                <div class="list__midfirst__vlaues">
                    <p>07 Oct 2018</p>
                    <p>Date</p>
                </div>
            </div>

            <div class="list__midfirst">
                <div class="list__midfirst__vlaues">
                    <p id="list__paid__vericaton">Paid</p>
                </div>
            </div>

            <div class="list__midfirst">
                <div class="list__midfirst__vlaues">
                    <img src="/img/eye.svg" alt="">
                </div>
            </div>
        </div>
    </div>    
</template>

<script>

export default {
  components: {
  
  
}
};
</script>

<style scoped>

.list_holder {
    
    display: flex;
    flex: 1;
    justify-content:space-between;
}


.list {
    margin-top:2px;
    display: flex;
    flex: 1;
    background-color: white;
    padding: 10px;
}

img {
    width: 20px;
    height: 20px;
    margin-right: 10px;
}

.list__start {
    display: flex;
}

.list__values > * {
    
    margin: 0;
    font-size:small;
    font-weight: lighter;
    letter-spacing: 1px;
}

.list__midfirst > div > *{
    margin: 0;
    font-size:small;
    font-weight: lighter;
    letter-spacing: 1px;    

}

#list__paid__vericaton{
    border: 1px solid greenyellow;
    padding-left: 5px;
    padding-right: 5px;
}

</style>
