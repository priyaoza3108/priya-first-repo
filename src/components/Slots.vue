<template>
    <h2>Slots</h2>
    <!-- For multiple slots -->
    <ChildSlots>
        <template v-slot:header>
            <h1>Html data in slots</h1>
        </template>
        <template  v-slot:content>
            <button>Buy Now</button>
        </template>
        <template  v-slot:footer>
            <p>A vue js product</p>
        </template>
        
    </ChildSlots>
    <!-- For Simple slots -->
    <!-- <ChildSlots><a href="#">Xyz</a></ChildSlots>
    <ChildSlots></ChildSlots>
    <ChildSlots><img src="https://images.unsplash.com/photo-1541963463532-d68292c34b19" height="200" width="200"/></ChildSlots> -->
</template>

<script>
import ChildSlots from './ChildSlots.vue';

export default{
    name: "Slots",
    components: { ChildSlots },
}
</script>