<template>
    <h3 v-for="name in names" :key=name.firstname>
        <slot :fristName="name.firstname"></slot>
        <slot :lastName="name.lastname"></slot>

    </h3>

</template>

<script>
    export default {
        name: "NameList",
        data() {
            return {
                names: [
                {
                    firstname: 'Bruce',
                    lastname: 'Wayne'
                },
                {
                    firstname: 'Clark',
                    lastname: 'Kent'
                },
                {
                    firstname: 'Princess',
                    lastname: 'Diana'
                }

                ],
            }
        }
    }
</script>

<style scoped>

</style>