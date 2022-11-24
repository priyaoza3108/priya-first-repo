<template>
    <!-- Parent to child -->
    <h2>{{ name }}</h2>
    <h2>{{ user.name }}</h2>
    <h2>{{ user.email }}</h2>
    <button v-on:click="getData()">Call Parent Function</button>

    <!-- Child to parent -->
    <button v-on:click="getUser(userName)">Send Name to Parent</button>

</template>

<script>
export default {
    name: 'Child',
    props: {
        name: String,
        user: Object,
        getData: Function,
        getUser: Function
    },
    data(){
        return{
            userName: "XYZ" 
        }
    }
}
</script>