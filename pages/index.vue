<template>
  <div class="container">
    <button id="login" @click="goToLogin"> Login Button</button>
    <button id="login" @click="goToDashboard"> Dashboard</button>

  </div>
</template>

<script>
  import {
    Component,
    mixins,
    Vue
  } from 'nuxt-property-decorator'


  export default {



    props:{
      screenID: {
        id:{ 
          type:String
        }
      }
    },


    methods: {
      goToLogin() {

        this.$router.push('/login')

      },
      goToDashboard() {
        this.$router.push('/dashboard')
      }
    }

  }
</script>

<style>
  body {
    background-color: rgb(163, 182, 218);
  }
</style>