<template>
    <h1>Dynamic Components</h1>
    <button @click="tab='Java'">Load Java</button>
    <button @click="tab='Php'">Load Php</button>
    <button @click="tab='Node'">Load Node</button>
    <component :is="tab"/>
</template>

<script>
import Java from './DynamicComponents/Java.vue';
import Node from './DynamicComponents/Node.vue';
import Php from './DynamicComponents/Php.vue';

export default{
    name: "DynamicComponent",
    provide: {
        message: "Provide/Inject Example"
    },
    components: { Java, Php, Node },
    data(){
        return{
            tab:''
        }
    }
}
</script>