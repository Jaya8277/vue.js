<template>
    <h2>Students Data</h2>
    <h3>Student name is : {{name}}</h3>
    
    </template>
    
    <script>
    export default {
        name: 'Student',   
        props:{
            name:String
        }
    }
    </script>
    