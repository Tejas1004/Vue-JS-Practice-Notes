<template>
    <div>
         <h1 v-if="error.length">Errorhandler type</h1>
         <ul>
            <li v-for="e in error" v-bind:key="e.id">{{e}}</li>
        </ul>
         
         <form @submit="validate"> 
            <input type="text" placeholder="Enter your Name" v-model="name"> <br> <br>
            <input type="password" placeholder="Enter Your Password" v-model="password"> <br> <br>
            <button  type="submit">Login</button>
         </form>
    </div>
</template>

<script>
export default {
    name: "ErrorHandle ",
    data(){
        return{
            error:[],
            name:null,
            password:null,
        }
    },
    methods:{
        validate(e){
            this.error = [];
            if(this.name && this.password){
                console.warn("its fine");
            }
            if(!this.name){
                this.error.push("Invalid name");
            }
            if(!this.password){
                this.error.push("Password required");
            }
            console.warn("Hi")
            e.preventDefault();
        }
    }
}
</script>