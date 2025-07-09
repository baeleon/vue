<script setup>
import Button from "@/stories/components/Buttons/Button.vue";
import Header from "@/stories/components/Header/Header.vue";
import router from "./router";

const clickFunction = () => {
      console.log("hello world");
};
</script>

<template>
      <Header />
      <RouterView />
      <Button size="small" :primary="true" title="Button" :onclick="clickFunction" />
      <Button size="small" title="Button 2" :onClick="() => router.push('/about')" />
</template>

<style scoped></style>
