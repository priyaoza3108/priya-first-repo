<template>
    <h1>Grand Child</h1>
    <h2>{{message}}</h2>
</template>

<script>
    export default{
        name:'InnerChild',
        inject:['message'],
    }
</script>