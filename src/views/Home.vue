<template>
  <div class="h-screen flex flex-col items-center justify-center">
    <h1 class="text-3xl tracking-wider text-indigo-500">Hello Electron!</h1>
    <p class="mt-5">
      This sample app included <strong>Vue3 + Typescript + TailwindCSS</strong>
    </p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import axios from "axios";

export default defineComponent({
  name: "Home",
  components: {},
  async setup() {
    const r = await axios.get("http://localhost:3000", {});
    console.log(r);
  },
});
</script>
