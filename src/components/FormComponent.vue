<template>
    <h2>Form</h2>
    <ul class="error">
        <li v-for="item in error" v-bind:key="item">
            {{item}} not valid
        </li>
    </ul>
    <form>
        <label>Email: </label>
        <input type="email" placeholder="Enter Email" v-model="formData.email" />
        <br /><br />
        <label>Password: </label>
        <input type="password" placeholder="Enter Password" v-model="formData.password" />
        <br /><br />
        <label>Country: </label>
        <select v-model="formData.country">
            <option>India</option>
            <option>USA</option>
            <option>China</option>
        </select>
        <br /><br />
        <h3>Technology: </h3>
            <label for="java">Java </label>
            <input type="checkbox" v-model="formData.technology" value="java" id="java" />

            <label for="php">PHP </label>
            <input type="checkbox" v-model="formData.technology" value="php" id="php" />

            <label for="node">Node </label>
            <input type="checkbox" v-model="formData.technology" value="node" id="node" />
        <br /><br />
        <h3>Gender: </h3>
            <label for="female">Female </label>
            <input type="radio" v-model="formData.gender" value="female" id="female" />

            <label for="male">Male </label>
            <input type="radio" v-model="formData.gender" value="male" id="male" />

        <br /><br />
        <button type="button" v-on:click="login()">Login</button>
    </form>
</template>

<script>
export default {
    name: 'FormComponent',
    data(){
        return{
            formData: {
                email:'',
                password:'',
                country:'',
                technology:[],
                gender:'',
            },
            error:[],
        }
    },
    methods:{
        login(){
            this.error=[];
            for(const item in this.formData){
                if(this.formData[item] === "" || this.formData[item].length === 0 ){
                    this.error.push(item);  
                }
            }
            if(this.error.length == 0){
                alert("Data submitted successfully");
            }
            console.log("Login Data",this.formData,this.error);
        }
    }
}
</script>

<style>
.error{
    color: rgb(233, 98, 98);
}
</style>