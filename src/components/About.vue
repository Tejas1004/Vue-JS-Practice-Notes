<template>
    <div>
        <h1>About components</h1>
        <Users />
        <Contact />
    </div>
</template>

<script>
import Contact from './Contact.vue';
import Users from "./users.vue";

export default {
    name:"About",
    components:{
        Users,
        Contact
    }
}
</script>

<style scoped>
    div{
        background-color: aqua;
        height: 500px;
    }
</style>