<template>
    <h1>{{childUser}}</h1>
    <Users :getUser="getUsersName"/>

</template>
<script>
import Users from './Users.vue'
export default {
    name:'Parent',
    data(){
        return {
            childUser:""
        }
    },
    components:{
        Users
       
    },methods:{
        getUsersName(name){
            // alert(name)
            this.childUser=name;
        }
    }
}
</script>