<template>
    <h1>If Else Rendering</h1>
    <h2 v-if="show">Show</h2>
    <h2 v-else >Hide</h2>
    <button v-on:click="show=!show">Toggle</button>
</template>

<script>
export default{
    name:'IfElse',
    data(){
        return{
            show: false
        }
    },
}
</script>