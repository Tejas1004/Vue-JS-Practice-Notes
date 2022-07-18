<template>
    <div>
        <!-- <h1>Hello Homie</h1> -->
        <!-- <h2>{{data}}</h2>
        <h2>{{ msg }}</h2> -->
        <!-- <button v-on:mouseover="hello('Hello call')">Push me</button> -->
        <!-- <h1 v-if="show">Conditional rendering using if block</h1>
        <h1 v-else>Conditional rendering using else block</h1>
        <button v-on:click="display"> Toggle Button</button> -->
       <h1>For Loop</h1>
       <table>
            <tr>
                <td>id</td>
                <td>name</td>
                <td>Email</td>
            </tr>
            <tr v-for="user in users" :key="user.id">
                <td>{{user.id}}</td>
                <td>{{user.name}}</td>
                <td>{{user.email}}</td>
            </tr>
       </table>
   
  
    </div>
</template>
<script>
export default {
    name: 'Home',
    props:{
        data:String,
        msg:String
    }
    // methods:{
    //     hello(data)
    //     {
    //         alert(data)
    //     }
    // }
    // ,data(){
    //     return {show:false}   
    // }
    // ,methods:{
    //     display(){
    //         this.show = !this.show;
    //     }
    // }

    ,data(){
        return{
            users:[
                {id:"1",name:"Tejas",email:"tejas@gmail.com"},
                {id:"2",name:"abjas",email:"abjas@gmail.com"},
                {id:"3",name:"cdjas",email:"cdjas@gmail.com"},
                {id:"4",name:"efjas",email:"efjas@gmail.com"},

            ]
        }
    }
}
</script>
