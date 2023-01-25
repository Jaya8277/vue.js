<template>
<h1>Pass data to child components</h1>
<Child name="Jaya" :users="users" :getData="getData" />
</template>

<script>
import Child from './Child.vue'
export default {
    name: 'PassDatatochild',
    components: {
        Child
    },
    data() {
        return {
            users: {
                name: "kiran",
                email: "kiran@gmail.com"
            }
        }
    },
    methods:{
        getData(){
            console.log("parent function called")
            alert("parent function called successfully")
        }
    }

}
</script>
