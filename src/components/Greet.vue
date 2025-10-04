<template>
    <div>
        <h1>Hello from Greet Component {{ name }} age{{ age }}</h1>
    </div>
</template>

<script>
    export default {
        name:  "Greet-Component" ,
        props: ['name','age']
    }
</script>

<style scoped>

h1 {
    color: blue;
}
</style>