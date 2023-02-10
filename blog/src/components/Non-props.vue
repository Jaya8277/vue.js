<template>
    <h1>Non-props Data</h1>

    <Nonuser data="some datas" id="user-cmp"/>
</template>
<script>
import Nonuser from './Nonuser.vue';
export default{
    name:"Non-props",
    components:{
        Nonuser
    }

}
</script>