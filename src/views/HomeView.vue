<template>
  <div class="home">
    <MdEditor :value="value" :handle-change="onchange" />
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App" />
  </div>
</template>

<script setup lang="ts">
import { defineComponent, ref } from "vue";
import HelloWorld from "@/components/HelloWorld.vue";
import MdEditor from "@/components/MdEditor.vue"; // @ is an alias to /src

const value = ref();
const onchange = (v: string) => {
  value.value = v;
};
</script>
