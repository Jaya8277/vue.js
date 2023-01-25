<template>
    <h2>Props Components</h2>
    <Student :name="name"/>
    <Teacher :name="name"/>
    </template>
    
    <script>
    import Student from './Student.vue'
    import Teacher from './Teacher.vue'

    export default {
        name: 'Props',   
        data(){
            return{
                name:"Kuhu"
            }
        },
        components:{
     Student,
     Teacher
        }
    }
    </script>
    