<template>
    <div>
        <h1 >{{name}}</h1>
        <button v-on:click="toggle">Destroy</button>
    </div>
</template>

<script>
export default {
    name:"Destroy",
    data(){
        return{
            name:"Hello"
        }
    },
    // methods:{
    //     toggle(){
    //         this.display=!this.display
    //     }
    // },
    beforeDestroy(){
        alert("before");
        console.warn("before Destroy")
    },
    destroyed(){
        alert("Destroy")
        console.warn("destroy")
    }
}
</script>