<template>
    <h1>Teleport Components</h1>
    <Teleport to="#footer">
        <Footer />
    </Teleport>
</template>

<script>
import Footer from './Footer.vue';

export default{
    name: "TeleportComp",
    components: { Footer }
}
</script>