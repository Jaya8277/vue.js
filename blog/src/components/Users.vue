<template>
<h1>Users data</h1>
<button v-on:click="getUser(userName)"> Send User name</button>
</template>

<script>
export default {
    name: 'Users',
    data() {
        return {
            userName: "jaya"
        }
    },
    props: {
        getUser: Function
    }

}
</script>
