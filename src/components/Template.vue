<template>
    <div >
        <p v-html="rowHtml"></p>
        <h2>Tejas</h2>
        <h2 v-once>{{name}}</h2>
        <h2>{{name}}</h2>
        <h2>{{ok?"true":"false"}}</h2>
        <button v-on:click="updateme">click</button>

    </div>
</template>

<script>
export default {
    name:"Template",
    data()
    {
        return {
            name:"Anil",
            ok:"true",
            rowHtml:"<h1>Template In Vue JS</h1>"
            
        }
    },
    methods:{
        updateme(){
            this.rowHtml = "<h1>Fuck you</h1>";
            
            
        }
    }
}
</script>
