<template>
    <div >
        <input type="text" placeholder="Enter Your Name" v-model="loginData.username"> <br> <br>
        <input type="text" placeholder="Enter Your Password" v-model="loginData.password"> <br> <br>
        <button v-on:click="loginData">Login</button>

    </div>
</template>

<script>
export default {
    name:"Form",
    methods:{
        loginData(){
            console.warn("Login Successfull")
        }
    },
    data()
    {
        return {loginForm:{
                username:null,
                password:null
            }}
        }
    
}
</script>
