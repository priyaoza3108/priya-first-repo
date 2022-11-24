<template>
    <h2>Class Bindiing</h2>
    <div :class="applyStyle">
        <h1>Test</h1>
    </div>
    <Button v-on:click="colorfull                                                                                                             =                                                                                                             !colorfull">Change Test Color</Button>
</template>

<script>
export default {
    name: 'ClassBinding',
    data() {
        return {
            colorfull: false
        }
    },
    computed: {
        applyStyle() {
            return {
                active: this.colorfull, err: true, other: true
            }
        }
    }
}
</script>
<style scoped>
.active {
    background-color: green;
    width: 200px;
}

.err {
    color: red;
}

.other {
    font-size: 20px;
}
</style>