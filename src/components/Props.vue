<template>
    <div >
        <h1>Props components</h1>
        <h2>{{ name }}</h2>
        <!-- <h1 v-for="user in value" :key="user.name">{{user.name}} "+"  {{user.email}}</h1> -->
        <table>
            <tr>
                <td>name</td>
                <td>Email</td>
            </tr>
            <tr  v-for="user in value" :key="user.name">
                <td>{{user.name}}</td>
                <td>{{user.email}}</td>
            </tr>
        </table>
    </div>
</template>

<script>
export default {
    name:"Props",
    props:['value']
}
</script>
