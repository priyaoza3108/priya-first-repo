<template>
    <!-- <h1 v-on:mousemove="getConsole()">test</h1> -->
    <button v-on:click="getData()">Click Me</button>
    <h2>Count : {{count}}</h2>
</template>

<script>
    export default{
        name: 'Event',
        data(){
            return {
                count : 0
            }
        },
        methods:{
            getData(){
                this.count++;
            },
            getConsole(){
                console.log("Event called")
            }
        }
    }
</script>