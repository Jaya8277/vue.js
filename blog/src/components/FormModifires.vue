<template>
    <h1>Form Modifires</h1>
    <input type="number" v-model.lazy.number.trim="data"/> <!--trim-->
    <h2>Data is : {{typeof(data)}}</h2>
</template>
<script>
export default{
    name:"FormModifires",
    data()
    {
        return {
            data:''
        }
    }
}
</script>