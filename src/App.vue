<script setup>
import ClassBinding from './components/ClassBinding.vue';
import DynamicComponent from './components/DynamicComponent.vue';
import Event from './components/Event.vue';
import ForLoopAndLists from './components/ForLoopAndLists.vue';
import FormComponent from './components/FormComponent.vue';
import GetInput from './components/GetInput.vue';
import HelloWorld from './components/HelloWorld.vue'
import Home from './components/Home.vue';
import HtmlBinding from './components/HtmlBinding.vue';
import IfElse from './components/IfElse.vue';
import Parent from './components/Parent.vue';
import Ref from './components/Ref.vue';
import Slots from './components/Slots.vue';
import TwoWayBinding from './components/TwoWayBinding.vue';
import Wathchers from './components/Wathchers.vue';
import TeleportComp from './components/TeleportComp.vue';
</script>

<template>
      <!-- <HelloWorld msg="You did it!" /> -->
      <!-- <Home /> -->
      <!-- <Event /> -->
      <!-- <TwoWayBinding /> -->
      <!-- <GetInput /> -->
      <!-- <IfElse /> -->
      <!-- <ForLoopAndLists /> -->
      <!-- <Parent /> -->
      <!-- <HtmlBinding /> -->
      <!-- <ClassBinding /> -->
      <!-- <Ref /> -->
      <!-- <FormComponent /> -->
      <!-- <Wathchers /> -->
      <!-- <Slots /> -->
      <!-- <DynamicComponent /> -->
      <!-- <TeleportComp /> -->
      
      <!-- Routing  -->
      <router-link to="/">Home</router-link> <br />
      <router-link to="/contact-us">Contact Us</router-link> <br />
      <router-link to="/about-us">About Us</router-link> <br />
      <router-link to="/profile/abc">ABC Profile</router-link> <br />
      <router-link to="/profile/xyz">XYZ Profile</router-link> <br />
      <router-link to="/profile/pqr">PQR Profile</router-link> <br />

      <router-view></router-view>

</template>