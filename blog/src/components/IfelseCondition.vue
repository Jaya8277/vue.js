<template>
    <h1 v-if="show">If else condition</h1>
    <!-- <h1 v-if="hide">If else condition1</h1> -->
    <h1 v-else>else condition</h1>
    <button v-on:click="show=!show">Toggle</button>
</template>
<script>
export default {
    name:'IfelseCondition',
    data(){
        return{
            show:true,
            hide:false
        }
    }
}
</script>