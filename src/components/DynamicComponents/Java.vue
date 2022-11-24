<template>
    <h1>Java Content</h1>
    <InnerChild />
</template>

<script>
import InnerChild from './InnerChild.vue';

    export default{
    name: "Java",
    components: { InnerChild }
}
</script>