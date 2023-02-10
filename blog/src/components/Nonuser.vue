<template>
  <div>  
    <h1 v-bind="$attrs">mongo Data</h1>
    <h2>react Data</h2>
    <h3>node Data</h3>
    <!-- <h1>{{data}}</h1> -->
</div>
</template>
<script>
export default{
    name:"Nonuser",
    inheritAttrs:false,//hide id
    props:{
       
        data:String
    }
    
}
</script>