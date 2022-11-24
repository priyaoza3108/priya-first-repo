<template>
    <h2>Parent Component</h2>
    <!-- Send data parent to child -->
    <!-- add : as prefix because we use data from data() and methods-->

    <Child name="Priya Oza" :user="user" :getData="getData" :getUser="getUserName"/>

    <!-- childUser is come from child component -->
    <!-- Basically it is send data child to parent -->

    <h3>{{childUser}}</h3>
</template>

<script>
import Child from './Child.vue';

export default{
    name: "parent",
    components: { Child },
    data(){
        return{
            user: {
                name: 'abc',
                email: 'abc@test.com'
            },
            childUser: ""
        }
    },
    methods: {
        getData(){
            console.log("Parent Fun called");
        },
        getUserName(name){
            this.childUser=name;
        }
    }
}
</script>