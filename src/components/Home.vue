<template>
    <h1>Home Page</h1>
    <!-- <h1>Name : {{getName("Abc")}}</h1>
    <h1>AllData : {{getData()}}</h1>
        <p>{{getData().name}}</p>
        <p>{{getData().email}}</p> -->
</template>

<script>
    export default{
        name: 'home',
        data(){
            return {
                email: 'abc@test.com',
            }
        },
        methods: {
            getName(name){
                return name;
            },
            getData(){
                return{
                    name: 'Priya Oza',
                    email: this.email
                }
            }
        }
    }
</script>
<style scoped>
h1{
    color: orange;
}
</style>