<template>
    <h1>Life Cycle in Vue</h1>
</template>

<script>
export default {
    name:"LifeCycle",
    data(){
        return{} 
    },
        created:function(){
            console.warn("Created");
        },
        beforeCreate:function(){
            console.warn("Before Create");
        },
        beforeMount:function(){
            console.warn("Before Mounted");
        },
        mounted:function(){
            console.warn("mounted");
        }
    
}
</script>