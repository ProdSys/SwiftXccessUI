<template>

  <div>
    <div :class="{ 'd-none': screen !== 0 }" class="form-screen">
      <RegisterForm :screenValue="screen" @Clicked="Clicked"></RegisterForm>
    </div>
    <div :class="{ 'd-none': screen !== 1 }" class="form-screen">
      <PersonalDetails ></PersonalDetails>
    </div>
  </div>

</template>


<script>
  import {
    Component,
    mixins,
    Vue
  } from 'nuxt-property-decorator'

   import    RegisterForm from '~/components/registration/RegistrationForm1';
   import    PersonalDetails from  '~/components/registration/PersonalDetails';
    
  
  export default  {

    components:{
RegisterForm,
PersonalDetails
    },

    data(){
      return {
        screen: 0,
      }
    },
    methods: {
      Clicked(){
      this.screen = 1;
    }

    },
  }
</script>