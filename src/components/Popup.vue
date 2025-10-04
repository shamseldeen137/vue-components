<template>
    <div>
<h2> this is PopUp</h2>
<input type="text" v-model="name" name="" id="">
<button @click="$emit('close',name)"> Close Pobup</button>
    </div>
</template>

<script>
    export default {
        name: "PopUp",
        emits:{
            close: (name) => {
                if(!name) return false;
            return true;
                }
        },
        data() {
            return {
            name: '',
            }
        }
    }
    


</script>

<style scoped>

</style>