<template>
    <h1>Form Modifires</h1>
    <input type="text" v-model.lazy="data"/>
    <h2>Data is : {{data}}</h2>
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