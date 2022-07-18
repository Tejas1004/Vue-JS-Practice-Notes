<template>
    <div>
        <h1 id="demo">Mounted on {{name}}</h1>
    </div>
</template>

<script>
export default {
    name:"Mount",
    data(){
        return{
           name:"Tejas",
        }
    },
    beforeMount(){
        console.warn(document.getElementById("demo"))
    },
    mounted(){
        console.warn(document.getElementById("demo"))
    }
}
</script>