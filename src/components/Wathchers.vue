<template>
    <h1>Watchers</h1>
    <button v-on:click="increment"> + </button>
    {{count}}
    <button v-on:click="decrement"> - </button>
</template>

<script>
export default{
    name:'Watchers',
    data(){
        return{
            count: 0    
        }
    },
    methods:{
        increment(){
            this.count++;
        },
        decrement(){
            if(this.count > 0)
                this.count--;
        }
    },
    watch: {
        count(val,prev){
            if(val>5 && val>prev){
                // alert("stop counting")
                this.count=0
            }
        }
    }
}
</script>