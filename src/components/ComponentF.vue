
<template>
    <div>
        <h2> component F</h2>
<h3>
    component F  {{ userName }}
</h3>
    </div>
</template>

<script>
    export default {
        name: "ComponentF",
        inject: ['userName'],
    }
</script>

<style scoped>

</style>