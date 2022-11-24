<template>
    <input type="text" v-model="text"/>
    <h2>Text : {{text}}</h2>
</template>

<script>
export default{
    name: 'TwoWayBinding',
    data(){
        return{
            text: 0
        }
    }
}
</script>