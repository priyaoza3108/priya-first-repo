<template>
    <h2>{{text}}</h2>
    <div v-html="tag"></div>
</template>

<script>
export default{
    name:'HtmlBinding',
    data(){
        return{
            text:'Abc xyz',
            tag:'<h1>Abc</h1>'
        }
    }
}
</script>