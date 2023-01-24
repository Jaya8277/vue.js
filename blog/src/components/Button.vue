<template>
    <h1 v-on:mousemove="getConsole()">onmouse</h1>
<button v-on:click="getData('button 1 clikked successs')">click me</button>
<button v-on:click="getData('button 2 clikked successs')">click me</button>
<button v-on:dblclick="getData('button dobule clikked successs')">click me</button>
<h1>{{count}}</h1>
<button v-on:click="getCount('button 1 clikked successs')">click me</button>
<button v-on:click="getCounts('button 2 clikked successs')">click me</button>
</template>
<script>
export default {
    name:'Button',
    data(){
return{
    count:0
}
    },
    methods:{
        getData(data){
            alert(data)
        },getConsole(){
            console.log("function run sucess")
        },
        getCount(){
            this.count = this.count +1
        },getCounts(){
            this.count=this.count - 1
        }
    }
}
</script>