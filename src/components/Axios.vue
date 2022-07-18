<template>
    <div>
        <h1 >Fetch Data from Axios</h1>
         <div>
            <table border="1px">
                <tr >
                     <td>Id</td>
                    <td>DishName</td>
                    <td>description</td>
                    <td>image</td>
                </tr>
                <tr v-for="data in list" v-bind:key="data.id">
                    <td>{{data.id}}</td>
                    <td>{{data.dishName}}</td>
                    <td>{{data.description}}</td>
                    <td>{{data.image}}</td>
                </tr>
            </table>
         </div>
    
    </div>
</template>

<script>
import Vue from 'vue';
import VueAxios from "vue-axios";
import axios from "axios";

export default {
    name:"Axios",
    data(){
        return{
            list:undefined
        }
    },
    mounted () {
    axios
      .get('https://raw.githubusercontent.com/syook/react-dishpoll/main/db.json')

      .then(response => {
        this.list = response.data
        // console.warn(response.data.data)
      })
  }
}
</script>