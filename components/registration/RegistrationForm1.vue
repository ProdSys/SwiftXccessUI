<template>

  <div id="mainOuter">
    <div id="div_companyRegister" class="container">
      <div id="innerDiv">
        <b-form @submit.prevent="onSubmit" @reset="onReset" v-if="show" class="form-group">
              <div><img src="/img/logo.svg" alt="" style="margin-bottom:10px;"></div>

          <b-form-group id="input-group-1"  label-for="input-1">
            <b-form-input size="lg" id="input-1" v-model="form.email" type="email" required placeholder="Enter email" width="200px">
            </b-form-input>
          </b-form-group>
          <b-form-input size="lg" type="password" placeholder="Enter your Password"></b-form-input>
          <b-form-group id="input-group-4">
            <b-form-checkbox-group v-model="form.checked" id="checkboxes-4">
              <b-form-checkbox value="me"><p style="color:white;">I accept the terms of use and privacy policy</p></b-form-checkbox>
            </b-form-checkbox-group>
          </b-form-group>

          <b-button 
          id="submintButton"
          type="submit"  variant="light">Continue</b-button>
        </b-form>

      </div>
    </div>
  </div>

</template>

<script>
  export default {
    
    props:{
      screenValue:{
        type:Number
      }
    },
    data() {
      return {
        form: {
          email: '',
          name: '',
          food: null,
          checked: []
        },
        show: true,
        screenValue2:this.screenValue
      }
    },
    methods: {
      onSubmit(){

        this.$emit('Clicked')
        
        
        console.log('submit');
        console.log(this.screenValue)
      },
      
      onReset(){
        console.log('reset');
      }
    },
  }
</script>



<style scoped>
  #div_companyRegister {
    text-align: center;
    position: absolute;
    width: 30%;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    padding: 1%;
    background-color:rgb(34, 34, 153);

    box-shadow: rgba(27, 17, 17, 0.4) 0 0 10px;
    border-radius: 50px 20px;

  }

#checkboxes-4{
margin-top: 10px;
text-align: left;
}


#input-1{
  margin-top: 30px;
}

#submintButton{
  box-shadow: rgba(27, 17, 17, 0.4) 0 0 10px;
    border-radius: 50px 20px;
}
</style>