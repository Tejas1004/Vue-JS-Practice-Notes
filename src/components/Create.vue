<template>
    <div>
        <h1>{{name}}</h1>
    </div>
</template>
<script>
export default {
    name: 'Create',
    data(){
        return{
            name:"Tejas",
        }
    },
    beforeCreate(){
        this.name = "dhjedh"
        console.warn("BeforeCreate",this.name)
    },
    created(){
    
        console.warn("Created",this.name)
    }
}
</script>