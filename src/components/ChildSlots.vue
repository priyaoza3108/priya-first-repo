<template>
    <!-- For Single Slot -->
    <!-- <slot><h1>Child component</h1></slot> -->
    <!-- For Multiple slot -->
   <div class="box">
        <header>
            <slot name="header"></slot>
        </header>
        <content>
            <slot name="content"></slot>
        </content>
        <footer>
            <slot name="footer"></slot>
        </footer>
   </div>
</template>

<script>
export default{
    name:'ChidSlot',
}
</script>

<style>
.box{
    border: 1px solid;
    width: 170px;
    text-align: center;
    padding: 20px;
}
</style>