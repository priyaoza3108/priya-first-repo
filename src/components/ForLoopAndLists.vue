<template>
    <h1>For Loops and Lists</h1>
    <ul>
        <li v-for="tech in technologies" :key="item">{{tech}}</li>
    </ul>
    <br /><br /><br />
    <ul>
        <li v-for="user in users" :key="user.name">
            Name: {{user.name}} and Email: {{user.email}}
        </li>
    </ul>
</template>

<script>
export default{
    name:'ForLoopAndLists',
    data(){
        return{
            technologies: ['java','php','node','html'],
            users: [
                {
                    name: 'priya',
                    email: 'priya@test.com'
                },{
                    name: 'abc',
                    email: 'abc@test.com'
                },{
                    name: 'xyz',
                    email: 'xyz@test.com'
                }
            ]
        }
    }
}
</script>