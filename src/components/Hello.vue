<template>
    <div>
        <div class="greeting">Hello {{name}}</div>
    </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
    props: ['name'],
});
</script>

<style scoped>
.greeting {
    font-size: 20px;
}
</style>
