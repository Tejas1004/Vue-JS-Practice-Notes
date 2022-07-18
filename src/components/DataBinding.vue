<template>
    <div >
        <h1>DataBinding components</h1>
        <h2 style="white-space:pre-line">{{message}}</h2>
        <textarea type="text" v-model="message"/>
    </div>
</template>

<script>
export default {
    name:"DataBind",
    data(){
        return{
            message:"Jack Ryan"
        }
    }
    
}
</script>
