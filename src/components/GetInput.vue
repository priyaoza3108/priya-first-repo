<template>
    <h1>Get Input Values</h1>
    <input type="text" placeholder="Enter Email" v-model="email"/>
    <br /><br />
    <input type="password" placeholder="Enter Password" v-model="password" />
    <br /><br />
    <h3>Known Technologies:</h3>
        <label for="java">Java</label>
        <input type="checkbox" value="java" id="java" v-model="technologies" />

        <label for="php">PHP</label>
        <input type="checkbox" value="php" id="php" v-model="technologies"/>

        <label for="node">Node</label>
        <input type="checkbox" value="node" id="node" v-model="technologies"/>
    <br /> <br />
    <h3>Gender:</h3>
        <label for="male">Male</label>
        <input type="radio" value="male" id="male" name="gender" v-model="gender"/>

        <label for="female">Female</label>
        <input type="radio" value="female" id="female" name="gender" v-model="gender" />
    <br /> <br />
    <button v-on:click="getData()" type="button">Get Values</button>
</template>
<script>
export default{
    name:'GetInputValue',
    data(){
        return{
            email:null,
            password: null,
            technologies: [],
            gender: null
        }
    },
    methods:{
        getData(){
            console.log("values: " +this.email +", "+this.password);
            console.log("technologies: " +this.technologies);
            console.log("gender: "+this.gender);
        }
    }
}
</script>