<template>
<h2>Child Components</h2>
<h1>{{name}}</h1>
<h1>{{users.name}}</h1>
<button v-on:click="getData">Call funtion</button>
</template>

<script>
export default {
    name: 'Child',
    props: {
        name: String,
        users: Object,
        getData:Function
    }
}
</script>
