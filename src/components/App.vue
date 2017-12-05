<template>
  <div>
    Name: <input v-model="name" type="text">

    <h1>Hello Component</h1>
    <hello :name="name" />

    <br>

    <h1>Hello Component JS</h1>
    <hello-js :name="name" />

  </div>
</template>

<script lang="ts">
import Vue from "vue";

import Hello from "@/components/Hello.vue";
import HelloJs from "@/components/HelloJs.vue";

export default Vue.extend({
    components: {Hello, HelloJs},
    data() {
        return {
            name: 'World',
        }
    }
});
</script>

<style scoped>
.greeting {
    font-size: 20px;
}
</style>
