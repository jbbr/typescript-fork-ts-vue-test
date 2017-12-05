<template>
    <div>
        <div class="greeting">Hello {{name}} from a JS module</div>
    </div>
</template>

<script>
export default {
    props: ['name'],
}
</script>

<style scoped>
.greeting {
    font-size: 20px;
    color: green;
}
</style>
