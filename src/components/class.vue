<template>
    <div class="homestyle">
        <h1>Class And style binding</h1>
        <h1 v-bind:style="{color:'blue'}"> style binding</h1>
        <h1 v-bind:class="{display:show}"> class binding with object</h1>
        <h1 v-bind:class="[aclass]"> class binding with array</h1>
        <h1 v-bind:class="[heroic ?'yes I am Hero':'No I am Not']"> class binding with object</h1>
    
    </div>
</template>
<script>
export default {
    name:"Class",
    data(){
        return{
            show:true,
            heroic: false,
            aclass : "arrayclass"
        }
    }
    
}
</script>
<style scoped>
    .homestyle{
         color: orange;
    }
    .display{
        background-color: brown;
    }
    .arrayclass{
        background-color: black;
    }
</style>