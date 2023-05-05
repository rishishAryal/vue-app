<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Say My Name" />
  <MyHome></MyHome>
  <NewComponent></NewComponent>
  <MyNewComponent></MyNewComponent>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import MyNewComponent from "@/components/MyNewComponent.vue";
import MyHome from "./components/MyHome.vue";
import NewComponent from "@/components/NewComponent.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    MyHome,
    NewComponent,
    MyNewComponent
  },
};
</script>
