<template>
<h1>Get Input Fields</h1>
<input type="text" placeholder="enter email" v-model="email"/>
<br/>
<br/>
<input type="password" placeholder="enter password" v-model="password" />
<br/><br/>
<button v-on:click="getData" type="button">Get Values</button>
</template>
<script>
export default {
    name:'GetInput',
    data(){
return{
    email:null,
    password:null
}
    },
    methods:{
        getData()
        {
            console.log("values:",this.email,this.password)
        }
    }
}
</script>
<style scoped>
h1{
    color:orange;
}
</style>