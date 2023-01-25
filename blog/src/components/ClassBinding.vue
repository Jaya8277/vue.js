<template>
<h1>Css Binding</h1>
<h2 :class="applyStyle">Home Components</h2>
<button v-on:click="colorfull=!colorfull">Apply Style</button>
</template>

<script>
export default {
    name: 'ClassBinding',
    data() {
        return {
            colorfull: true
        }
    },
    computed:{
        applyStyle(){
            return {
                green:this.colorfull,
                err:true,
                other:false
            }
        }
    }
}
</script>

<style>
.green {
    background-color: green;
    width: 200px;
    padding: 10px;

}
.err{
    color:red;
}
.other{
    font-size:50px;
}
</style>
