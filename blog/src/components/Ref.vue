<template>
<h2>Ref in vue js</h2>
<input type="text" ref="input" />
<button v-on:click="getData">Click Me</button>
</template>

<script>
export default {
    name: 'Ref',
    methods: {
        getData() {
            
            this.$refs.input.focus();
            let val =  this.$refs.input.value;
            console.log(val)
            this.$refs.input.style.color="red";
        }
    }
}
</script>

<style>
</style>
