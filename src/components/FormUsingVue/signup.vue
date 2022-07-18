<template>
    <div>
        <input type="text" placeholder="Enter Your name" v-model="signup.username"> <br> <br>
        <input type="password" placeholder="Enter Your Password" v-model="signup.password"><br> <br>
        Choose Hobbies <br> <br>
        <input type="checkBox" id="cricket"  v-model="signup.hobbies">
        <label for="cricket">Cricket</label>
        <input type="checkBox" id="football" v-model="signup.hobbies">
        <label for="football">Football</label>
        <br> <br>
        Choose Gender <br> <br>
        <input type="radio" id="male" value="male" v-model="signup.gender">
        <label for="male">Male</label>
        <input type="radio" id="female" value="female" v-model="signup.gender">
         <label for="female">Female</label>
         <br> <br>
         <button v-on:click="signupUser">Register User</button>
        <br> <br>
        
    </div>
  
</template>
<script>

export default {
    name:"Signup",

    data(){
        return{
            signup:{
                username:null,
                password:null,
                hobbies:[],
                gender:null
            }
        }
    },
    methods:{
        signupUser(){
            console.warn(this.signup);
        }
    }
}
</script>