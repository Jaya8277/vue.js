<template>
<h1>Home Components {{10+20}}</h1>
<h1>Home Components {{"Hello".length}}</h1>
<h1>Email{{email}}</h1>
<h1>Mobile{{mobile}}</h1>
<h1>Name{{getName()}}</h1>
</template>
<script>
export default {
    name:'Home',
    data(){
        return{
            email:"jaya@gmail.com",
            mobile:86789867,
            getName:function(){
                return "Jaya Vishwakarma"
            }
        }
    }
}
</script>
<style scoped>
h1{
    color:orange;
}
</style>